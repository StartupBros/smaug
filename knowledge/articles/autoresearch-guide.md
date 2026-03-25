# Autoresearch Guide

**Source:** https://www.aibyaakash.com/p/autoresearch-guide
**Author:** Aakash Gupta
**Topic:** Using Karpathy's autoresearch framework for iterative optimization

## Overview

Aakash Gupta's comprehensive guide to using Karpathy's open-sourced autoresearch framework. For $25 and a single GPU, you can run 100 experiments overnight without designing any of them.

## Key Concepts

The autoresearch architecture uses three files:
1. **program.md** - Human writes strategy in plain English
2. **train.py** - Agent executes, iterates, and ships code
3. **val_bpb** - Locked evaluation layer (neither human nor agent can modify mid-run)

## The Core Insight: Immutable Evaluation

The critical pattern is separating goal-setting from evaluation. The agent optimizes against a locked metric that it cannot redefine, adjust, or game. This prevents the metric from drifting and ensures improvements are real.

### Real-World Results

- **Karpathy's ML work:** Found 20 improvements in hand-optimized code, achieving 11% speedup
- **Shopify (Tobi Lutke):** 53% faster Liquid template rendering from 93 automated commits
- **Large model transfer:** 20 proven improvements on a 2x larger model all transferred successfully

## Six Use Cases

The guide covers applying this pattern to:
- Ad copy optimization
- Cold email sequences
- Video scripts
- Job posts
- Skill files
- (and others)

## The Setup

Three-step setup with evaluation mistakes to avoid. Each optimization cycle takes 5 minutes: Score up → Git commit. Score down → Git reset. 12 cycles per hour, 100+ overnight.

## Scaling to Organizations

The principle extends to organizational structures:
- **Sales:** Agent writes sequences, independent system scores replies, human sets targeting
- **Product:** Agent ships variants, locked analytics measure retention, PM writes experiment brief
- **Recruiting:** Agent screens candidates, calibrated rubric scores them, hiring manager defines role

## The Principle

"Whoever controls the eval controls the outcome. Lock it down or the agent will find the shortest path to a number that means nothing."
