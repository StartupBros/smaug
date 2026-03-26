---
title: "zeroclaw"
type: tool
date_added: 2026-02-15
source: "https://github.com/theonlyhennygod/zeroclaw"
tags: []
via: "Twitter bookmark from @geekbb"
---

ZeroClaw is a personal AI assistant built in Rust as a lightweight alternative to OpenClaw. It runs on channels you already use (Telegram, WhatsApp, Slack, Discord, Signal, and more) with dramatically lower resource usage: 3.4MB binary vs OpenClaw's 28MB, and just 7.8MB RAM vs 1.52GB — a 194x reduction. Designed for self-hosting on minimal hardware (including $10 devices like Raspberry Pi and Arduino), it supports model-agnostic backends and connects to hardware peripherals via ESP32/STM32/Arduino.

## Key Features

- 100% Rust implementation — zero overhead, minimal binary size
- Supports 20+ messaging channels including WhatsApp, Telegram, Slack, Discord, Signal, iMessage, Matrix, IRC, Reddit, LinkedIn, Twitter, and more
- Web dashboard for real-time control
- Hardware peripheral support (ESP32, STM32, Arduino, Raspberry Pi)
- Migration path from OpenClaw via `zeroclaw onboard` command
- Runs on <5MB RAM — claimed 99% less memory than OpenClaw

## Links

- [GitHub](https://github.com/theonlyhennygod/zeroclaw)
- [Original Tweet](https://x.com/geekbb/status/2022846202581258585)
