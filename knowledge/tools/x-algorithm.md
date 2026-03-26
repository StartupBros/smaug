---
title: "x-algorithm"
type: tool
date_added: "2026-01-20"
source: "https://github.com/xai-org/x-algorithm"
tags: []
via: "Twitter bookmark from @fomomofosol"
---

X's open-sourced For You feed recommendation engine, built in Rust and powered by a Grok-based transformer model. It retrieves candidate posts from both in-network (accounts you follow, via Thunder) and out-of-network sources (ML-based global corpus retrieval, via Phoenix), then ranks them by predicted engagement probability. Notable for having eliminated hand-engineered features entirely — the transformer handles all scoring from engagement history.

## Key Features

- Grok-based transformer scoring (ported from xAI's Grok-1 release)
- Two candidate pipelines: Thunder (in-network) and Phoenix (out-of-network retrieval)
- Home Mixer orchestration layer managing query hydration, hydration, and filtering
- Engagement-history-driven ranking with no manual feature engineering
- Written in Rust with 16k+ stars at time of bookmark

## Links

- [GitHub](https://github.com/xai-org/x-algorithm)
- [Original Tweet](https://x.com/fomomofosol/status/2013566879625847142)
