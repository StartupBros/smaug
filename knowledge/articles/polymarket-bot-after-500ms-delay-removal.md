---
title: "How to build a Polymarket bot (after new rules edition)"
type: article
date_added: 2026-02-21
source: "https://x.com/i/article/2024859635878871040"
author: "dominatos"
tags: []
via: "Twitter bookmark from @PolymarketStory"
---

A technical guide to building Polymarket prediction market bots under the new rules introduced in early 2026. On February 18, 2026, Polymarket silently removed the 500ms taker delay on crypto markets and introduced dynamic taker fees on 5-minute and 15-minute crypto markets (up to 1.56% at 50% probability). These changes broke most existing bots and killed pure taker arbitrage strategies.

The new meta is maker-side liquidity provision: makers pay zero fees and earn USDC rebates funded by taker fees. The article explains WebSocket-based orderbook streaming (replacing REST polling), fee-aware order signing (the `feeRateBps` field that must match the current rate or orders are rejected), and fast cancel/replace loops targeting under 100ms cycle time. For 5-minute BTC up/down markets specifically, the strategy is to post maker orders at T-10 seconds before window close when direction is ~85% determined but Polymarket odds haven't fully priced it in.

## Key Takeaways

- The 500ms delay removal and dynamic taker fees fundamentally changed Polymarket bot economics — taker arb from 2025 is now unprofitable
- Maker bots earn rebates as their primary profit source; zero fees + USDC rebates is the new baseline
- WebSocket orderbook streams are mandatory; REST polling is too slow post-delay-removal
- `feeRateBps` must be included in signed order payloads; omitting it causes order rejection on fee-enabled markets
- Query fee rates dynamically before every order — never hardcode
- For 5-min BTC markets: price Binance direction faster than other makers and post at 90-95¢ on the winning side 10 seconds before close
- Fast Rust clients (polyfill-rs, polymarket-hft) offer significant latency advantages over the official Python SDK

## Links

- [Article](https://x.com/i/article/2024859635878871040)
- [Original Tweet](https://x.com/PolymarketStory/status/2025189132763385926)
