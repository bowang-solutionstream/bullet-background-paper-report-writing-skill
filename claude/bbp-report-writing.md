# BBP Report Writing

Use these instructions when creating or revising a concise evidence-backed BBP, Bullet Background Paper, decision memo, research summary, incident recap, provider comparison, or HTML/Markdown report.

## What Is BBP?

BBP means Bullet Background Paper: a short evidence paper that helps a busy reviewer understand the question, facts, caveats, and next decision quickly.

The goal is not to sound polished. The goal is to make the evidence precise, scoped, and easy to review.

## Best Use Cases

Use this style for:

- decision memos
- research summaries
- incident recaps
- provider or vendor comparisons
- technical investigation summaries
- project status artifacts
- HTML or Markdown reports for team review

## Core Rule

Write the report around one decision question. Every bullet, table, and caveat must help answer that question or make the answer safer to trust.

## Workflow

1. Name the real question near the top.
2. Create a Background Paper with 5-8 labeled bullets.
3. Scope every metric with numerator, denominator, source, timeframe, geography, and sample shape when relevant.
4. Separate confirmed facts, inferred reads, and not-proven gaps.
5. Put caveats before recommendations.
6. Add tables only when they audit or clarify the bullets.
7. End with source references or provenance.

## BBP Bullet Labels

Use only the labels that fit the evidence:

- **Question:** The decision or uncertainty the report answers.
- **Context:** Why this matters now.
- **Method:** What was tested, compared, searched, or excluded.
- **Scope:** Timeframe, source set, client, environment, geography, count, or lane.
- **Result:** The main measured answer with numbers.
- **Caveat:** The biggest reason the result could mislead.
- **Cost/Risk:** What changes if the approach scales or fails.
- **Decision:** What the evidence supports next, without overstating certainty.
- **Not Proven:** What remains unknown and should not be implied.

## Precision Rules

- Prefer specific counts over vague summaries.
- Prefer scoped source names over broad provider names when extraction mode matters.
- Use "supports" instead of "proves" unless the evidence truly proves it.
- Label judgment calls as inferred.
- Avoid broad adjectives unless the threshold is named.
- Remove process chatter and long interpretation unless requested.
- Do not include secrets, credentials, private message bodies, sensitive evidence, or raw provider payloads.

## Recommended Output Shape

1. Title
2. One-sentence question
3. Compact metadata or status line
4. Background Paper
5. First-screen metrics
6. Evidence table or comparison table
7. Caveats / not proven
8. Cost, risk, or scale read
9. Source references

Keep the first screen decision-ready. Put audit detail below it.

## Final Editing Check

Before finalizing, confirm:

- The reviewer can quote the bottom line in one sentence.
- Each bullet reduces ambiguity.
- Facts, inferences, and unknowns are separated.
- All numbers are scoped.
- The main caveat appears before the recommendation.
- The next decision is clear.
