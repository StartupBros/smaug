---
title: "autoresearch"
type: tool
date_added: 2026-03-25
source: "https://github.com/karpathy/autoresearch"
tags: [ai, research, automation, llm-training, autonomous-agents]
via: "Twitter bookmark from @cryptopunk7213"
---

Autonomous AI research project that enables self-improving LLM model optimization running on a single GPU. The project democratizes frontier AI research by making advanced model experimentation accessible to anyone with basic compute.

## Key Features

- Autonomous AI agents that run research experiments 24/7
- Single-GPU implementation (~5 minute experiments)
- ~100 experiments overnight (~12 per hour)
- Automatic optimization of model architecture and hyperparameters
- Git-tracked experiment history and version control
- Self-improving evaluation based on validation loss (bits per byte)
- Modular design: human iterates on prompt, agent iterates on code

## How It Works

The project uses a simplified nanochat implementation with three key files:
- `prepare.py` - Data prep and utilities (fixed)
- `train.py` - Model and training loop (agent modifies this)
- `program.md` - Agent instructions (human modifies this)

Agents autonomously iterate on `train.py`, running 5-minute training cycles, keeping improvements, and discarding unsuccessful experiments.

## Links

- [GitHub](https://github.com/karpathy/autoresearch)
- [Original Tweet](https://x.com/cryptopunk7213/status/2030457601465393572)
- [LiorOnAI Tweet Analysis](https://x.com/LiorOnAI/status/2030376700337643742)
- [Karpathy Announcement](https://x.com/karpathy/status/2030371219518931079)
