<!--
File: README.md
Core: Public GitHub landing page for the DaE product repository and distribution entrypoints.
Input: Final positioning, benchmark summary, SSRN link, and distribution targets.
Output: English README suitable for the repository root, including the canonical Skills CLI package path after duplicate-package cleanup.
-->

# DaE: Persona Context Injector

**Profile first. Then collaborate.**

[中文说明](./README.zh-CN.md)

DaE is an upstream context layer for the agent era.

It uses structured questioning to generate a reusable `PersonaProfile`, so downstream agents can understand the user before they start planning, coding, writing, researching, or advising.

## Why DaE exists

Most AI workflows fail for the same reason:

**the model starts acting before it understands who it is working for.**

Users repeat themselves.
Agents guess.
Output becomes generic.

DaE fixes that by building a reusable profile once, then letting every downstream agent read it first.

## What DaE does

DaE does three things:

1. Elicit a high-fidelity persona through structured questioning
2. Produce a reusable `PersonaProfile`
3. Let downstream agents read that profile before doing work

DaE is not:

- a therapy bot
- a one-off personality quiz
- a generic prompt trick
- a direct advice engine

DaE is:

- a reusable profile generator
- a context injection layer
- a protocol for better downstream collaboration

## What makes DaE different

DaE does not simply collect self-description.

It is designed to:

- challenge vague identity labels
- force concrete events instead of abstract traits
- test claimed values against actual trade-offs
- surface tensions, decision style, and constraint logic

The output is not a pretty summary.
It is a reusable operating profile.

## Benchmark

Public demos do not use real private user profiles.

### Framework validation case

The first validation case uses **Steve Jobs** as a public historical subject to test whether DaE's question framework produces structured, dimension-rich profiles through elicitation.

**Methodological scope:** Steve Jobs is extensively documented in model training data. The model holds independent prior knowledge about him. The comparison below shows how a structured profile focuses a response — but cannot cleanly isolate the elicitation effect from the model's prior knowledge. This case validates the **question framework design and output structure**, not the downstream injection effect in isolation.

A clean injection test requires a profile built from a real user's live dialogue, where the model has no prior knowledge of that person.

Question used:

**How should Steve Jobs rebuild Apple after returning to the company?**

**Tested with:** `deepseek-chat` on `2026-03-14`

```diff
- WITHOUT PROFILE
- Steve Jobs should immediately refocus Apple on a simplified, high-quality product line, forge a strategic partnership with Microsoft for investment and software support, and launch innovative, consumer-friendly products like the iMac to re-establish the brand's premium identity and financial health.

+ WITH DAE PROFILE
+ Jobs should rebuild Apple by cutting aggressively before he tries to heal anything. Shrink the product line, concentrate authority around a small number of product decisions, and force the company back to end-to-end ownership of the user experience. He should not optimize for broad internal comfort or stakeholder consensus, because Apple's recovery in his hands would come from restoring product coherence and a single standard of taste.
```

More detail:

- [Benchmark write-up](./benchmark/Steve-Jobs.md)
- [Benchmark profile](./benchmark/Steve-Jobs-profile.md)

### Real-user elicitation

When DaE runs on a real user — someone the model has no prior knowledge of — the profile is built entirely from live dialogue responses. That is the intended operating mode.

Anonymous sample outputs from real elicitation sessions will be added here as they are cleared for publication.

## Research foundation

DaE is grounded in the research paper:

**Dialogue as Elicitation: A Framework for High-Fidelity Persona Profiling in Human-AI Collaboration**  
https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5961054

Related research repository:

https://github.com/sirsws/DaE-Personal-Strategic-Asset

This repository contains the operational implementation and release assets.  
The SSRN paper and research repository remain the methodology and academic reference sources.

## What the output looks like

A valid DaE profile includes structured fields such as:

- `Background`
- `Capabilities`
- `Resources`
- `Constraints`
- `Drives`
- `Goals`
- `DecisionStyle`
- `Weaknesses`
- `Tensions`
- `Lessons`
- `AlignmentCheck`

This is a reusable configuration asset, not a motivational essay.

## Distribution

DaE can be distributed in three forms:

- as a `ClawHub / OpenClaw` skill
- as a `Skills CLI / skills.sh` skill
- as an `agent-store` onboarding agent
- as a protocol integrated into custom agent workflows

## Install

Install from the repository with the Skills CLI:

```bash
npx skills add https://github.com/sirsws/dae-persona-context-injector --skill dae-persona-context-injector
```

The canonical Skills CLI-compatible package lives at:

- [Skills package](./skills/dae-persona-context-injector/SKILL.md)

Draft copy:

- [ClawHub skill page](./docs/clawhub-copy.md)
- [Agent-store landing copy](./docs/agent-store-copy.md)

## Security and boundaries

- DaE does not make final decisions for the user
- DaE does not disguise profiles as action plans
- DaE does not treat personality labels as evidence
- public demos use non-sensitive benchmark subjects
- real user profiles should be treated as local private configuration assets

## Status

Current stage:

- positioning finalized
- first benchmark completed
- ClawHub / GitHub / agent-store release assets published
- Skills CLI-compatible package structure added
- ClawHub live, OpenClaw marked Benign, VirusTotal clean

## One-line summary

DaE is an upstream context layer for agents:
build the profile first, then let every downstream agent work from a stronger starting point.
