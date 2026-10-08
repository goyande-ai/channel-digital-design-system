# Channel Digital Design System

Shared brand guidelines, assets, and components for Channel Digital — a web design, hosting and SEO agency in Truro, Cornwall.

This system covers proposal and quote decks, but is extensible to all presentations and client-facing designs.

## Quick Start

- **Guidelines:** See [BRAND.md](BRAND.md) for full brand specifications
- **Logos:** `assets/logos/` — mark and full wordmark in PNG format
- **Colors & Typography:** [tokens.json](tokens.json) — canonical design tokens
- **Components:** `components/` — reusable slide layouts and previews

## Structure

```
├── BRAND.md                 # Complete brand guidelines
├── tokens.json              # Design tokens (colors, typography, spacing)
├── design-system.json       # System metadata (Figma/design tool compatible)
├── assets/
│   ├── logos/               # Channel Digital logo (mark & full)
│   ├── backgrounds/         # Cover background geometric patterns
│   └── badges/              # Google five-star badge
├── components/
│   ├── cover/               # Cover slide layout & preview
│   ├── content/              # Content slide layout & preview
│   └── testimonial/         # Testimonial slide layout & preview
└── docs/
    └── implementation/      # How to use this system in projects
```

## Usage

### Copy into a project
```bash
cp -r assets components tokens.json /path/to/your/project/
```

### Reference in Claude Code
When starting a design or presentation project, reference the BRAND.md and tokens.json files for consistency.

## Brand Overview

**Tone:** First person plural, plain and warm. British spelling, no emoji.

**Colors:**
- `white` — background
- `grey` — text (5.1:1 on white)
- `red` — brand accent (logo)
- `red-dark` — dates and highlights
- `teal` — links (always underlined)
- `grey-pale` — strip headers

**Typography:**
- Open Sans (titles & body) — from Google Fonts
- Raleway (labels) — from Google Fonts
- Lato (slide numbers) — from Google Fonts

**Layout:** 16:9 slides, minimal design, square corners, no shadows or gradients.

## Logo Usage

- `channel-logo-mark.png` — mark only (used on every slide)
  - Top right of cover strip: 34px wide
  - Above content slide titles: 52px wide
  
- `channel-digital-logo.png` — full logo with wordmark
  - Use where the company name must appear
  - Place on white or grey-pale only
  - Do not recolour, resize, or redraw

## Updating This System

When the agency updates brand assets or guidelines:
1. Update the relevant files in `assets/`
2. Update `tokens.json` and `BRAND.md` to reflect changes
3. Commit and push to the main branch
4. Notify all projects to re-sync

## Sharing with Your Team

This design system is meant to be referenced across all Claude Code projects and presentations. Share the link to this repository or the BRAND.md file with anyone creating Channel Digital materials.

---

**Last updated:** 2026-10-08  
**Maintained by:** Pete Graves  
**Source:** Channel Proposal Template 2026
