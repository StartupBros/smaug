---
date: 2026-03-25
topic: video-podcast-transcription
---

# Video/Podcast Transcription

## Problem Frame

Smaug already categorizes YouTube, podcast, and video bookmarks into `transcribe` action categories with dedicated templates and knowledge directories. But the transcription step is unimplemented — these bookmarks produce placeholder files with `status: needs_transcript` and "*Pending transcription*" instead of real content. The README explicitly flags this as wanted ("PRs welcome!").

Users who bookmark videos and podcasts get second-class knowledge files compared to articles and GitHub repos, which are fully extracted and summarized.

## Requirements

- R1. Add transcript extraction to the fetch phase (`processor.js`) following the existing content extraction pattern (`fetchGitHubContent`, `fetchArticleContent`). Transcript text lands in the `content` field of each link, just like article HTML and GitHub README content do today.
- R2. For YouTube URLs, try caption/subtitle download via yt-dlp first (auto-generated or manual captions). This is the fast path — no audio download or Whisper needed.
- R3. If captions are unavailable and Whisper is installed, fall back to downloading audio with yt-dlp and transcribing with Whisper.
- R4. If neither captions nor Whisper are available, degrade gracefully to the current placeholder behavior (`status: needs_transcript`). Log a message suggesting Whisper installation for better coverage.
- R5. The `process-bookmarks.md` command uses transcript content to write rich knowledge files (summary, key takeaways, context) — the same way it uses article HTML to write article knowledge files. No change to the template structure needed; Claude just receives transcript text instead of "*Pending transcription*".
- R6. Zero new required dependencies. Both yt-dlp and Whisper are optional, detected at runtime. If neither is installed, transcribe-category bookmarks produce the current placeholder behavior — existing functionality is completely unchanged. This matches the bird CLI pattern (optional/detected).
- R7. Support non-YouTube video/podcast URLs where yt-dlp can extract audio (Vimeo, podcast direct MP3 links, etc.). Same tiered strategy: captions first, Whisper fallback, placeholder last resort.

## Success Criteria

- With no new tools installed: existing behavior is 100% unchanged (zero-risk merge)
- With yt-dlp installed: bookmarking a YouTube video with available captions produces a fully-written knowledge file (not a placeholder) on the next `smaug run`
- With yt-dlp + Whisper installed: bookmarking a podcast episode with no captions produces a transcribed knowledge file
- Missing tools produce the current placeholder file with a helpful log message — no crash, no hang
- The feature adds zero workflow changes for existing users — `smaug run` handles everything

## Scope Boundaries

- No new CLI commands (no `smaug transcribe`). Transcription happens inline during the fetch phase.
- No cloud/paid transcription APIs. Only local tools (yt-dlp, Whisper).
- No audio file persistence. Audio is a temporary artifact used only during transcription, then cleaned up.
- No transcript persistence. The raw transcript is an intermediate input to Claude's knowledge file generation, not a stored artifact (matching how raw HTML is handled for articles).
- No GUI or interactive transcript editing.

## Key Decisions

- **Inline in fetch phase, not a separate command**: Follows the existing architectural pattern where `processor.js` extracts content by link type. Videos/podcasts are no different from articles or GitHub repos — they just have a different extraction method.
- **Tiered strategy (captions > Whisper > placeholder)**: Optimizes for the common case (YouTube with captions) while supporting the long tail. Zero required dependencies — everything is optional and detected.
- **Graceful degradation over hard requirements**: Both yt-dlp and Whisper are optional. The PR is zero-risk to merge — without either tool installed, behavior is identical to today. With yt-dlp, ~95% of YouTube videos get transcripts. With Whisper added, coverage extends to captionless content.
- **Transcript as intermediate artifact**: Follows the article pattern — raw content is input to Claude's synthesis, not a stored output. This avoids file bloat and keeps knowledge files scannable.

## Dependencies / Assumptions

- yt-dlp is optional; detected at runtime like bird CLI. If missing, transcribe bookmarks produce placeholders.
- Whisper (openai-whisper Python package) is optional; enhances coverage for captionless content
- yt-dlp subtitle extraction works for the vast majority of YouTube videos (auto-generated captions)
- The process-bookmarks.md command already handles the `transcribe` action — it just needs transcript content in the link's `content` field to produce rich files instead of placeholders

## Outstanding Questions

### Deferred to Planning

- [Affects R2][Needs research] Which yt-dlp flags produce the cleanest caption text? (--write-sub vs --write-auto-sub, subtitle format preference, language selection)
- [Affects R3][Needs research] Which Whisper model size balances quality vs speed for typical bookmark content? (tiny, base, small, medium, large)
- [Affects R3][Technical] Chunking strategy for long audio files (1hr+ podcasts) with Whisper — process as one file or split?
- [Affects R1][Technical] How to handle subtitle format parsing (VTT timestamps, SRT formatting) to produce clean transcript text
- [Affects R7][Technical] Which non-YouTube platforms does yt-dlp reliably support for subtitle/audio extraction?
- [Affects R1][Technical] Timeout configuration for transcription during fetch — should it be configurable in smaug.config.json?
- [Affects R5][Technical] Does `process-bookmarks.md` need any template updates, or does the presence of transcript content in the `content` field naturally produce rich files via Claude's existing instructions?

## Next Steps

-> `/ce:plan` for structured implementation planning
