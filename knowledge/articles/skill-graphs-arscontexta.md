# Skill Graphs > SKILL.md

- **Source:** https://x.com/i/article/2023918991673061376
- **Author:** @arscontexta (Heinrich)
- **Date:** February 17, 2026

## Summary

Argues that single-file skills are insufficient for complex domains. Proposes "skill graphs" — networks of small interconnected markdown files linked via wikilinks — enabling agents to traverse only relevant knowledge nodes rather than loading monolithic files.

## Core Concept

A **skill graph** is a network of skill files connected with wikilinks. Instead of one big file, you have many small composable pieces that reference each other. Each file is one complete thought, technique, or skill.

Key properties:
- Every node has YAML frontmatter with a description the agent can scan without reading the full file
- Every wikilink carries meaning because it's woven into prose
- Progressive disclosure: `index → descriptions → links → sections → full content`
- Most decisions happen before reading a single full file

## Primitives

- **Wikilinks** written as prose in sentences — carry meaning not just references
- **YAML frontmatter** with descriptions — enables scanning without reading
- **MOCs** (Maps of Content) — organize clusters of related skills into navigable sub-topics

## Index Structure

The index file is an entry point that points attention, not a lookup table. It describes the landscape so the agent follows relevant links.

## Use Cases

- Trading skill graph: risk management, market psychology, position sizing, technical analysis
- Legal skill graph: contract patterns, compliance, jurisdiction specifics, precedent chains
- Company skill graph: org structure, product knowledge, processes, onboarding, culture
- Therapy skill graph: CBT patterns, attachment theory, active listening, emotional regulation

## arscontexta Plugin

A Claude Code plugin (~250 connected markdown files) that teaches an agent how to build skill graphs / knowledge bases. Uses `/learn` and `/reduce` skills.

The plugin covers: cognitive science, zettelkasten, graph theory, agent architecture — each piece linked, composable, traversable.

## How to Build One

**Easy way:** Install arscontexta Claude Code plugin, pick the research preset, point it at a topic. Sets up folder structure, then fill with `/learn` and `/reduce`.

**Manual way:** A skill graph doesn't need to live in `.claude/skills/`. The key is an index file that tells the agent what exists and how to traverse it.

## Key Insight

This is the difference between an agent that follows instructions and an agent that understands a domain. Skill graphs are context engineering — instead of one injection, the agent navigates a knowledge structure, pulling in exactly what the current situation requires.
