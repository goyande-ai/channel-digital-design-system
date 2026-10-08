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

## For Designers & Developers: Contributing

This design system is a living resource. If you notice gaps, inconsistencies, or improvements needed:

### Making Changes

1. **Clone the repo:**
   ```bash
   git clone https://github.com/goyande-ai/channel-digital-design-system.git
   cd channel-digital-design-system
   ```

2. **Make your changes:**
   - Update `BRAND.md` if guidelines need clarifying or expanding
   - Update `tokens.json` if colors, typography, or spacing change
   - Add/update assets in `assets/` with matching README files
   - Update `.claude/skills/channel-digital/SKILL.md` if reference material changes

3. **Commit and push:**
   ```bash
   git add -A
   git commit -m "Brief description of what changed and why"
   git push origin master
   ```

4. **Notify the team** that an update is available

### Common Updates

- **New logo or asset:** Add to appropriate folder in `assets/`, create/update README
- **Brand guideline change:** Update `BRAND.md` with the new rule and its rationale
- **Color/type change:** Update `tokens.json` AND `BRAND.md`, tag as a version bump
- **New component or layout:** Add to `components/` with preview and documentation

### Version Bumps

When making significant updates:
1. Tag the commit: `git tag v1.1` (or v2.0 for major changes)
2. Push tags: `git push origin --tags`
3. Update changelog in this README

### Questions or Suggestions?

Leave an issue in this repository, or comment on the [Claude Docs artifact](https://claude.ai/code/artifact/02e5b43d-262a-4e61-abf6-697e47513f47).

## Sharing with Your Team

**For everyone:** Share the [Claude Docs guide](https://claude.ai/code/artifact/02e5b43d-262a-4e61-abf6-697e47513f47) — it's readable and needs no GitHub access.

**For non-technical users:** Point them to the Docs link above and the "For Non-Technical Users" section there.

**For designers and developers:** Invite them as collaborators on this repository so they can contribute improvements.

---

**Last updated:** 2026-10-08  
**Maintained by:** Pete Graves  
**Repository:** https://github.com/goyande-ai/channel-digital-design-system  
**Source:** Channel Proposal Template 2026
