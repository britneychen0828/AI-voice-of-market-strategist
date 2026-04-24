# Signal Taxonomy

This document defines how `voice-of-market-strategist` should classify, weight, and interpret input signals before writing a report or deck.

## Why This Exists

The skill often receives messy, mixed-source input:

- firsthand user comments
- support issues
- purchase questions
- community takes
- benchmark debates
- launch-note claims
- translated or repeated comments

Without a stable taxonomy, the model will overcount noise, confuse vendor claims with user proof, or promote dramatic anecdotes into strategy.

## Primary Signal Buckets

Every deduplicated signal must have exactly one primary bucket.

### 1. Firsthand User Experience

Definition:
The speaker describes what they personally tried, saw, felt, or experienced.

Examples:
- "It fixed UI tweaks in my Electron app."
- "I had to restart sessions when the context window filled."
- "I preferred it without reasoning mode."

Use:
- strongest source for Product and Technology conclusions
- strong source for acquisition, retention, or switching-friction insights when behavior is explicit

### 2. Bug Or Support Issue

Definition:
The speaker reports a failure, blocker, defect, outage, or access problem.

Examples:
- "The API key returns 401 after payment."
- "Too many people trying please upgrade."
- "The trial was unusable because of portal rate limits."

Use:
- strongest source for reliability, onboarding, activation, and retention-risk conclusions

### 3. Purchase Or Pricing Question

Definition:
The speaker is evaluating whether to buy, run, or adopt the product and asks about cost, hardware, or access.

Examples:
- "How many Mac Studios do I need to run this locally?"
- "What are the costs and how do they compare?"

Use:
- directional source for demand, buying friction, and positioning
- weaker than firsthand use when assessing product quality

### 4. Community Opinion Or Benchmark Commentary

Definition:
The speaker gives an opinion, interpretation, or benchmark reaction that may or may not be grounded in personal usage.

Examples:
- "Benchmarks can be bloated and misleading."
- "KIMI K2.6 IS BENCHMAXED."

Use:
- useful for messaging risk, positioning skepticism, and narrative context
- should not be treated as direct proof of product reality

### 5. Official Or Vendor Claim

Definition:
The signal originates from release notes, benchmark charts, company case studies, or community retellings of those materials.

Examples:
- "The announcement says Agent Swarm expanded from 100 to 300."
- "The release notes say it refactored a financial engine for 13 hours."

Use:
- can provide context for what the company is trying to communicate
- must not be presented as equivalent to firsthand validation
- should generally be labeled low-confidence unless independently corroborated

### 6. Unknown / Ambiguous

Definition:
The signal cannot confidently be placed into another bucket.

Use:
- preserve cautiously
- do not overweight in conclusions

## Stance Labels

Each signal should also receive one stance label:

- Positive
- Negative
- Mixed
- Neutral / observational

This is useful for balance and for identifying tension.

## Confidence Levels

### High Confidence

Use when:
- multiple distinct firsthand or bug/support signals point in the same direction
- the claim is close to what users directly said

Examples:
- API access failures are blocking evaluation
- reasoning mode feels overthought and inefficient

### Medium Confidence

Use when:
- the pattern is plausible and supported, but not broad
- there are limited firsthand signals or meaningful counter-signals

Examples:
- switching cost from Kimi ecosystem matters
- session continuity is an issue, but evidence volume is modest

### Low Confidence

Use when:
- the claim comes mainly from vendor narrative, benchmark debate, or very thin signal volume
- the theme is interesting but not yet well-supported

Examples:
- agent swarm scale as a proven strength
- local model demand as a major roadmap priority from one or two questions

## Deduplication Rules

### Treat As Duplicates Or Near-Duplicates

- exact repeated comments
- bilingual restatements of the same idea
- truncated/full versions of the same post
- obvious paraphrases that preserve the same underlying signal

### Treat As Distinct

- separate users expressing the same pain point independently
- one comment about speed and another about reasoning loops, even if both are negative

## Consensus, Tension, And Severity

These are not the same thing.

### Consensus

Use only when:
- a clear multi-signal pattern exists
- counter-signals are weak or limited
- the language can honestly support "broad agreement"

### Tension

Use when:
- users split on quality, speed, value, or comparisons
- one segment reports a strength while another reports a weakness

### High Severity

Use when:
- a smaller cluster of signals points to a painful issue with large impact

Important:
High severity does not automatically equal consensus.

## Roadmap Gating

A theme qualifies for the roadmap when it is:

- high-confidence or strong medium-confidence
- meaningfully supported by the evidence
- strategically important

Themes that are interesting but thin should go to:

- Watchlist
- Open questions
- Future opportunities

They should not be promoted into a top-priority roadmap just to fill space.

## Quote Policy

Quotes must be exact substrings of the input.

Do not:
- fix grammar
- merge two quotes
- shorten text inside quotes unless the remaining substring is still exact
- translate and then quote

If you need to summarize, paraphrase without quotation marks.
