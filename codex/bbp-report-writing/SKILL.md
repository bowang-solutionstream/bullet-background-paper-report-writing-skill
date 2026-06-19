---
name: bbp-report-writing
description: Use when creating or revising concise evidence-backed BBP, Bullet Background Paper, decision memo, research summary, investigation artifact, provider comparison, incident recap, or HTML/Markdown report that must be precise, scoped, and review-ready.
---

# BBP Report Writing

## Overview

BBP means Bullet Background Paper: a short evidence paper that lets a busy reviewer understand the question, facts, caveats, and next decision quickly. Use it to turn dense investigation notes into a precise review artifact without adding a teaching layer.

## Core Rule

Write the report around one decision question. Every bullet, table, and caveat must help answer that question or make the answer safer to trust.

## Workflow

1. **Name the question.** Put the real question near the top as a sentence, not a topic label.
2. **Build the Background Paper first.** Use 5-8 labeled bullets. Choose only labels that fit the evidence.
3. **Scope every metric.** Include numerator, denominator, time window, provider/source, geography, and sample shape when relevant.
4. **Separate certainty levels.** Keep confirmed facts, inferred reads, and not-proven gaps distinct.
5. **Show caveats before action.** Make the main failure mode or limitation visible before any recommendation.
6. **Add evidence tables only after the BBP.** Tables should audit the bullets, not replace them.
7. **End with source/provenance.** Link artifacts, docs, issue/PR references, or command outputs used.

## BBP Bullet Jobs

Use this menu; do not force every label.

| Label | Job |
| --- | --- |
| Question | The decision or uncertainty the artifact answers. |
| Context | Why this matters now. |
| Method | What was tested, compared, searched, or excluded. |
| Scope | Timeframe, source set, client, environment, geography, count, or lane. |
| Result | The main measured answer with numbers. |
| Caveat | The biggest reason the result could mislead. |
| Cost/Risk | What changes if the approach scales or fails. |
| Decision | What the evidence supports next, without overstating certainty. |
| Not Proven | What remains unknown and should not be implied. |

## Precision Rules

- Prefer "11 / 120 rows" over "some rows".
- Prefer "Ahrefs per-source extraction" over "Ahrefs results" when the extraction mode matters.
- Prefer "supports testing X next" over "proves X".
- Use "inferred" for judgment calls that are not directly proven by evidence.
- Avoid broad adjectives such as strong, weak, promising, meaningful, or successful unless the threshold is named.
- Remove process chatter, motivational language, and long interpretation unless the user asks for it.
- Do not include secrets, raw credentials, private message bodies, sensitive evidence, or full provider payloads.

## Recommended Artifact Shape

For HTML or Markdown artifacts:

1. Title
2. One-sentence question
3. Status chips or compact metadata
4. Background Paper
5. First-screen metrics
6. Evidence table or comparison table
7. Caveats / not proven
8. Cost, risk, or scale read
9. Source references

Keep the first screen decision-ready. Put audit detail below the first screen.

## Editing Pass

After drafting, tighten with these checks:

- Can the reviewer quote the bottom line in one sentence?
- Does each bullet reduce ambiguity?
- Are facts, inferences, and unknowns separated?
- Are all numbers scoped?
- Is the caveat visible before the recommendation?
- Would a teammate know what to do next without reading raw notes?
- Is anything included mainly because it was interesting rather than decision-useful?

## Common Mistakes

- Starting with narrative history instead of the decision question.
- Mixing branded recall, unaided visibility, and provider capability as if they are one metric.
- Hiding the operational caveat in a source appendix.
- Saying "the data shows" without naming the sample and source.
- Overwriting uncertainty with confidence language.
- Adding a concept primer by default. Use a separate mentoring skill only when the user asks for knowledge-gap teaching.
