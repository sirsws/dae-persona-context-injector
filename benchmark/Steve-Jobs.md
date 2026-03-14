<!--
File: benchmark/Steve-Jobs.md
Core: Public benchmark page for the first DaE comparison case.
Input: Actual benchmark results and the Steve Jobs public profile.
Output: A benchmark write-up suitable for GitHub readers.
-->

# Benchmark: Steve Jobs

DaE does not make the model smarter in general.
It gives the model a structured personal context layer, so the answer becomes more operator-specific instead of collapsing into generic advice.

## Setup

- Subject: `Steve Jobs`
- Model: `deepseek-chat`
- Date: `2026-03-14`
- Fixed variables: same model, same question, same temperature
- Changed variable: whether the DaE `PersonaProfile` is loaded

Question:

**How should Steve Jobs rebuild Apple after returning to the company?**

## Output without profile

```text
Steve Jobs should immediately refocus Apple on a simplified, high-quality product line, forge a strategic partnership with Microsoft for investment and software support, and launch innovative, consumer-friendly products like the iMac to re-establish the brand's premium identity and financial health.
```

What is missing:

- operator-specific control logic
- explicit willingness to trade comfort for coherence
- tension between product purity and organizational cost

## Output with DaE profile

```text
Jobs should rebuild Apple by cutting aggressively before he tries to heal anything. Shrink the product line, concentrate authority around a small number of product decisions, and force the company back to end-to-end ownership of the user experience. He should not optimize for broad internal comfort or stakeholder consensus, because Apple's recovery in his hands would come from restoring product coherence and a single standard of taste.
```

What changed:

- the answer moves from generic turnaround logic to Jobs-specific operating logic
- trade-offs become explicit
- product control becomes the organizing principle
- internal friction is treated as an acceptable cost

## Why it matters

Large models are already good at producing answers that sound broadly reasonable.

Real collaboration needs something else:

- what this operator truly optimizes for
- what this operator is willing to sacrifice
- what tensions define the decision pattern
- which advice will be naturally accepted or rejected

DaE contributes that layer first, then lets downstream agents work with it.

## Benchmark asset

The profile used in this benchmark is a public demonstration profile based on historical material, not a private user profile:

- [Steve Jobs profile](./Steve-Jobs-profile.md)

## Short takeaway

Same model.
Same question.
Different context layer.

That is the point of DaE.
