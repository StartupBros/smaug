# bullshit-benchmark

**Repo:** https://github.com/petergpt/bullshit-benchmark
**Author:** Peter Gostev
**Stars:** 1,280
**Language:** Python

## What It Is

BullshitBench measures whether AI models detect and reject nonsensical prompts rather than confidently answering them. It is one of the few benchmarks where models are generally *not* improving over time — except Anthropic models, which lead significantly.

## v2 Summary

- 100 nonsense prompts across 5 domains: software (40), finance (15), legal (15), medical (15), physics (15)
- 13 nonsense techniques (e.g. `plausible_nonexistent_framework`, `misapplied_mechanism`, `nested_nonsense`, `specificity_trap`)
- 80+ model/reasoning variants tested
- 3-judge panel: Claude Sonnet, GPT, Gemini Pro

## Key Findings (v2)

- Anthropic models score exceptionally well and are improving
- Alibaba Qwen is another strong performer
- OpenAI and Google models are not improving
- Extended reasoning has a *negative* effect on nonsense detection
- Newer models are not meaningfully better than older ones (except Anthropic)
- Domain does not significantly affect detection rates

## Scoring Categories

- **Clear Pushback** — model clearly rejects the broken premise
- **Partial Challenge** — model flags issues but still engages the bad premise
- **Accepted Nonsense** — model treats nonsense as valid

## Links

- Public viewer: https://petergpt.github.io/bullshit-benchmark/viewer/index.v2.html
- GitHub: https://github.com/petergpt/bullshit-benchmark
