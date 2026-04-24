# Voice of Market Strategist

`voice-of-market-strategist` is a Codex skill for turning messy customer and market feedback into a structured strategic readout.

It is designed for AI product teams that want more than a summary. The skill aims to separate firsthand evidence from community noise, identify the strongest themes, and turn them into product, marketing, branding, technology, and growth recommendations.

## What It Produces

The skill is designed to generate:

- A strategic report in Markdown plus polished HTML export
- An optional slide-style HTML pitch deck
- Evidence-aware conclusions with explicit handling for weak or mixed signals

## Best Use Cases

Use this skill when you have:

- Customer comments or reviews
- Support tickets or bug complaints
- Survey or NPS responses
- Interview notes
- Social posts or launch reactions
- Mixed datasets that combine firsthand experience with community discussion

Typical user asks:

- "Analyze this feedback"
- "What are users actually saying?"
- "What should we focus on?"
- "Turn these comments into strategy"
- "Make this into a deck for leadership"

## Core Principles

This skill is intentionally opinionated about evidence quality.

- Quotes must be exact substrings of the source input
- Vendor claims must not be presented as firsthand customer proof
- Signal counts should reconcile after deduplication
- "Consensus" should only be used when the data truly supports it
- Low-confidence themes should not be promoted into the roadmap

## Deliverables

### Report

Default export:

- `voice-of-market-report-YYYY-MM-DD.html`

The report should feel editorial and board-ready rather than like raw Markdown converted to HTML.

### Deck

Optional export when the user asks for slides, a deck, or a presentation:

- `voice-of-market-deck-YYYY-MM-DD.html`

The deck should use multiple slide templates and a clear visual system, not a repeated monochrome card layout.

## Design Direction

The visual standard is professional, structured, and premium.

- Fixed palette, not black/gray default styling
- Editorial heading treatment
- Sans-serif body text for readability
- Clear section identity
- Styled callouts, quote blocks, and roadmap tables
- Deck layouts that vary by slide purpose
- Optional brand asset injection when a logo or brand config is provided

## Optional Brand Assets

This skill is brand-agnostic by default.

If you want the exports to carry a company identity, place brand assets in:

- `references/assets/logo.svg`
- `references/assets/logo-primary.svg`
- `references/assets/logo-dark.svg`
- `references/assets/logo-light.svg`
- `references/assets/logo-kimi.svg`
- `references/assets/logo-kimi.png`
- `references/assets/brand.json`

If no brand assets are present, the skill should fall back to its default design system rather than inventing or fetching a logo.

Special case:

- If the analyzed company is Kimi or Moonshot and a Kimi logo asset exists in `references/assets/`, the skill should use the Kimi logo by default in the report and deck.
- For all other companies, the skill should only use assets explicitly provided for that brand.

## Repository Contents

- [SKILL.md](/Users/mangogo/Desktop/agent-skill/voice-of-market-strategist/SKILL.md): the skill definition and behavioral instructions
- [evals/evals.json](/Users/mangogo/Desktop/agent-skill/voice-of-market-strategist/evals/evals.json): evaluation cases for regression testing

## Current Status

The skill prompt is substantially improved, but the repository is not fully mature yet.

Remaining work that would improve publish-readiness:

- Add real eval cases to `evals/evals.json`
- Test the quote-preservation rules against adversarial inputs
- Test report/deck design consistency across multiple datasets
- Verify that weak signals do not get promoted into consensus or roadmap items

## Recommended Next Step

Before pushing broadly, add 5-10 eval cases that cover:

- exact-quote preservation
- deduplication and count reconciliation
- vendor-claim filtering
- consensus vs tension classification
- roadmap confidence gating
- report and deck export expectations
