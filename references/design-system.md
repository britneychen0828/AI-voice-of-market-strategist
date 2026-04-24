# Design System

This document defines the visual system for `voice-of-market-strategist` exports.

The goal is not "pretty enough." The goal is to create outputs that feel structured, executive-ready, and intentionally designed.

## Design Principles

### 1. Professional, Not Generic

The report and deck should not look like default browser styling, raw Markdown, or a one-click AI export.

### 2. Editorial Clarity

The report should feel readable and authoritative, like a polished strategy memo or board note.

### 3. Presentation Rhythm

The deck should feel like a real narrative presentation with pacing, contrast, and slide variety.

### 4. Restrained Visual Identity

Use a small number of colors, type roles, and layout motifs consistently.

## Shared Palette

Use these as the default visual tokens.

### Core Colors

- Ink: `#172033`
- Secondary ink: `#314158`
- Accent blue: `#2563eb`
- Accent teal: `#0f766e`
- Warm emphasis: `#f59e0b`
- Surface: `#ffffff`
- Canvas: `#f5f7fb`
- Muted border: `#dbe4f0`
- Soft blue tint: `#eef4ff`
- Soft teal tint: `#ecfeff`
- Soft warm tint: `#fff7e6`

### Color Rules

- Do not rely on black and gray alone
- Use one dominant accent and one secondary accent
- Use warm emphasis only for warnings, watchlists, or high-attention states
- Keep backgrounds light and presentation-friendly

## Typography

## Report Typography

- Heading stack: `Iowan Old Style`, `Georgia`, `"Times New Roman"`, serif
- Body stack: `Inter`, `"Segoe UI"`, `Arial`, sans-serif
- H1: large editorial headline
- H2: section headline with accent treatment
- Body: readable, neutral, steady

## Deck Typography

- Slide titles: same serif stack or a strong display-feeling fallback
- Body and labels: modern sans-serif
- Use clear role separation:
  - title
  - support copy
  - label / metadata
  - caption / evidence

## Report System

### Report Layout

- Centered reading column
- 860px to 980px content width
- Generous outer spacing
- White reading surface on soft canvas background

### Required Components

- Title block
- Metadata row
- Executive summary callout
- Section dividers
- Editorial quote blocks
- Styled tables
- Confidence or evidence emphasis treatment when useful

### Report Styling Rules

- H1 should feel like a cover title, not a default app heading
- H2s should use a visible accent system: side bar, top rule, or section label
- Tables should have clear header fill, row striping, and breathing room
- Quote blocks should look curated, not browser-default
- Callouts should use tinted backgrounds and accent borders

### Report Anti-Patterns

- black/gray-only styling
- plain underlined headings as the only hierarchy device
- equal styling across all sections
- cramped spacing
- raw Markdown rendered with minimal cleanup

## Deck System

### Slide Composition

A 10-slide deck should use at least 3 distinct template types.

Recommended set:

- Title slide
- Big-idea slide
- Evidence quote slide
- Metrics/stats slide
- Two-column comparison slide
- Roadmap slide
- Closing recommendation slide

### Slide Layout Rules

- Keep strong top-level hierarchy
- Preserve generous whitespace
- Use large titles with concise support copy
- Avoid placing all content in the same repeated white card pattern
- Use accent areas, section dividers, stat clusters, or split layouts to create pacing

### Slide Visual Rhythm

- Title slide can be bolder and cleaner
- Big-idea slides should center one argument
- Evidence slides should use quotes or proof snippets prominently
- Stats slides should emphasize 1 to 3 numbers only
- Roadmap slides should privilege action, confidence, and timing over dense prose

### Deck Anti-Patterns

- monochrome black/gray slides
- every slide using identical card shells
- memo paragraphs pasted into slides
- thin accent bars with no deeper visual system
- decorative shapes that do not help comprehension

## Component Guidance

### Executive Summary Callout

Use:
- tinted surface
- accent border or accent top rule
- tighter typography than body copy

Avoid:
- plain gray box
- oversized paragraph blob with no emphasis

### Quote Blocks

Use:
- editorial left rule or inset block
- softer background
- slightly smaller or italicized body

Avoid:
- browser-default `blockquote` styling
- giant quote walls with no curation

### Tables

Use:
- clearly styled header row
- row striping or subtle separators
- strong first column or key-value emphasis

Avoid:
- spreadsheet look
- dense borders everywhere

### Confidence Tags

Use:
- restrained pill or label styling
- color mapping that is consistent across report and deck

Suggested mapping:
- High: blue or dark ink
- Medium: teal or muted blue-gray
- Watchlist / caution: warm amber

## Tone Through Design

The visual tone should suggest:

- strategic clarity
- trustworthiness
- calm authority
- product sophistication

It should not suggest:

- hype
- generic AI branding
- dashboard clutter
- startup template randomness
