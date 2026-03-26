---
title: "I Built an AI Company with OpenClaw + Vercel + Supabase - Two Weeks Later, They Run It Themselves"
type: article
date_added: 2026-02-06
source: "https://x.com/i/article/2019906747750658049"
author: "Vox (@Voxyz_ai)"
tags: []
via: "Twitter bookmark from @Voxyz_ai"
---

A detailed technical walkthrough of building a fully autonomous multi-agent system (VoxYZ Agent World) with 6 AI agents running a live website. The author goes from "agents can talk" to "agents run the website end-to-end" in two weeks using OpenClaw on a VPS, Next.js/Vercel for the control plane, and Supabase as shared state. The core insight is that bridging agent output to actual execution requires a closed feedback loop: propose → auto-approve → create mission+steps → execute → emit event → trigger reaction → repeat.

Three pitfalls are documented in detail: (1) a race condition when both VPS and Vercel tried to claim the same tasks — fixed by making VPS the sole executor; (2) triggers creating proposals that never progressed to missions because the auto-approve and mission-creation steps were skipped — fixed with a single `createProposalAndMaybeAutoApprove` function all paths must call; (3) proposals generating queued steps even when quotas were already full — fixed with a Cap Gates system that rejects at the proposal entry point rather than letting work pile up silently. A reaction matrix stored in the policy table introduces probability-based inter-agent responses, giving the system non-deterministic behavior that feels more like a team than a robot. The heartbeat route handles stale task recovery for self-healing under network/VPS instability.

## Key Takeaways

- Designate a single executor (VPS); let Vercel only run the lightweight control plane (evaluate triggers, process reactions, recover stale tasks)
- All proposal-creation paths must funnel through one function that enforces cap gates, auto-approve, and mission/step creation atomically
- Cap gates reject at proposal time, not at execution time — prevent queue buildup rather than cleaning it up later
- Probability-based reaction rules (e.g., 30% chance an agent analyzes a posted tweet) make multi-agent systems feel emergent rather than mechanical
- `recoverStaleSteps` in the heartbeat marks running tasks failed after 30 minutes of no progress, enabling genuine self-healing
- Architecture: OpenClaw (think + execute) / Vercel (approve + monitor) / Supabase (all shared state)

## Links

- [Article](https://x.com/i/article/2019906747750658049)
- [Original Tweet](https://x.com/Voxyz_ai/status/2019914775061270747)
