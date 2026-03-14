<!--
File: docs/clawhub-copy.md
Core: Draft ClawHub skill page copy for the DaE release.
Input: Final English positioning and benchmark summary.
Output: Publishable copy for ClawHub or OpenClaw submission.
-->

# DaE ClawHub Skill Page Draft

## Skill Title

**DaE: Persona Context Injector**

## One-line Description

Generate a reusable PersonaProfile that downstream agents can read before planning, coding, writing, researching, or advising.

## Short Description

DaE is a front-loaded profiling skill for the agent era.

It does not give life advice.
It builds a structured user profile that forces concrete events, trade-offs, constraints, and tensions into a reusable asset.

Run it once.
Let downstream agents read the profile first.
Get less generic output afterward.

## What It Solves

Most agents fail for the same reason:

**they start working before they understand who they are working for.**

DaE fixes that by generating a reusable profile containing:

- goals
- constraints
- trade-offs
- tensions
- decision style
- weakness triggers

This is not a personality quiz.
This is an upstream context layer.

## What Makes DaE Different

DaE does not accept self-description at face value.

It is designed to:

- challenge soft identity labels
- force concrete events instead of vague traits
- ask what the user actually gave up to preserve a claimed value
- output tensions and decision logic that downstream agents can use

The result is not a motivational summary.
The result is a reusable operating profile.

## Benchmark

**Subject:** Steve Jobs  
**Tested with:** `deepseek-chat` on `2026-03-14`  
**Question:** How should Steve Jobs rebuild Apple after returning to the company?

```diff
- WITHOUT PROFILE
- Steve Jobs should immediately refocus Apple on a simplified, high-quality product line, forge a strategic partnership with Microsoft for investment and software support, and launch innovative, consumer-friendly products like the iMac to re-establish the brand's premium identity and financial health.

+ WITH DAE PROFILE
+ Jobs should rebuild Apple by cutting aggressively before he tries to heal anything. Shrink the product line, concentrate authority around a small number of product decisions, and force the company back to end-to-end ownership of the user experience. He should not optimize for broad internal comfort or stakeholder consensus, because Apple's recovery in his hands would come from restoring product coherence and a single standard of taste.
```

Same model. Same question. Different context layer.

## Security Notes

- local profile generation
- no unrelated system privileges
- public demos use non-sensitive benchmark profiles

Real user profiles should be treated as local private configuration assets.

## Closing Line

**Profile first. Then collaborate.**
