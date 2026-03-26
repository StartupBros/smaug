---
title: "How to Sell to Agents"
type: article
date_added: 2026-02-16
source: "https://x.com/i/article/2023464512964489218"
author: "brian flynn (@Flynnjamm)"
tags: []
via: "Twitter bookmark from @Flynnjamm"
---

A rigorous economic analysis of how AI agents change the buyer/seller relationship, starting from Coase's 1937 transaction costs theorem and updating it for a world where search and evaluation costs approach zero. The core argument: when an agent can discover, price, and call a service in a single HTTP roundtrip, the economics of buy-vs-build completely change. Agents aren't attention-seeking consumers — they query, optimize for outcomes, and make purchasing decisions based on speed and cost, not brand recognition.

The article identifies the key asymmetry: a GPT-4-class model reasoning about "what scraping services exist?" costs $0.10–0.50 and takes 10–25 seconds; a specialized catalog service returns the same answer for $0.01–0.02 in under 200ms. That's 7–50x cheaper and 50–100x faster. When speed matters (because pipeline latency compounds), specialization beats generalization almost every time. This creates economic room for hyper-specialized single-endpoint services that would never sustain a subscription model but thrive on fractions of a cent per call.

The product requirements for agent-native services are fundamentally different: pricing must be in the API response (not a webpage), onboarding must be fully programmable (no dashboard clicking), and reliability becomes the entire product — in one survey of 44 agent services, only 2 had fully working endpoints. HTTP 402 (Payment Required), dormant since 1997, becomes the standard mechanism for machine-readable pricing.

## Key Takeaways

- Agents don't browse — they query, so your marketing site and pricing page are invisible at runtime
- Discovery must be programmatic: machine-readable capability registries that return structured data (what you do, what it costs, how to pay)
- A specialized service at $0.01/call beats a general agent spending 25 seconds reasoning about the same sub-task
- The new sales funnel is: get on the agent's allowlist (human decision), then win on price/speed/reliability at runtime
- HTTP 402 Payment Required is finally finding its intended use: machine-readable per-request pricing in API responses
- Reliability is existential: dead or inaccurate services get zero traffic permanently — agents route around them
- Services with proprietary data, real-time feeds, or hardware-dependent computation have durable moats; pure reasoning services get absorbed as models get cheaper
- The three-call onboarding ideal: one to discover, one to authenticate, one to buy — no humans in the loop

## Links

- [Article](https://x.com/i/article/2023464512964489218)
- [Original Tweet](https://x.com/Flynnjamm/status/2023465136204419096)
