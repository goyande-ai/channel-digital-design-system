# Channel Digital Brand Helper

A guide to applying Channel Digital brand guidelines consistently across all presentations, designs, and client-facing materials.

## What This Skill Does

When invoked, this skill helps you:
- Apply brand voice and tone to proposal copy
- Select and use colours correctly for accessibility
- Choose the right typography and sizing for different contexts
- Build layouts that follow the grid and spacing rules
- Use logos correctly (mark vs. full logo, sizing, placement)
- Check your work against the brand guidelines

## How to Use

Reference this skill when:
- Creating a new proposal or presentation deck
- Writing client-facing copy or testimonials
- Designing a new slide layout or component
- Choosing colours, fonts, or imagery
- Building an extension or variation of the system

## Quick Reference

**Brand voice:** First person plural, plain and warm, British spelling
**Colours:** white background, grey text, red accents (brand red #ed1b32), teal links (#3d8aa7)
**Typography:** Open Sans (titles & body), Raleway (labels), Lato (numbers)
**Layout:** 16:9 canvas, 720 × 405px source, top-left aligned, no shadows/gradients/borders
**Logos:** Mark on every slide (34px cover, 52px content); full logo where name must appear

## Source Files

All brand definitions, tokens, and assets live in the **channel-digital-design-system** project:

- `BRAND.md` — Complete brand guidelines with detailed usage rules
- `tokens.json` — Design tokens (colors, typography, spacing) for developers
- `assets/` — Logo files, backgrounds, and badges
  - `logos/channel-logo-mark.png` — 34px on cover, 52px on content
  - `logos/channel-digital-logo.png` — Full logo with wordmark
  - `backgrounds/cover-background-geometric.png` — Cover background
  - `badges/google-five-star-badge.png` — Google five-star for testimonials

## Brand Guidelines at a Glance

### Voice & Tone
- "Let us know if you'd like to chat further." (first person plural)
- "I look forward to hearing from you." (closing)
- Capitalize cover elements (COMPANY NAME, PROPOSAL TITLE, DATE)
- Title case for everything else ("Project Overview", "Next Steps")
- British spelling, no emoji
- Full testimonial quotes with attribution: "Quote here." (Name, Company)

### Colours
| Use | Colour | Hex |
|-----|--------|-----|
| Slide background | white | #ffffff |
| Text (titles, body) | grey | #6d6e71 |
| Top strip (content) | grey-pale | #e9edee |
| Accents, shapes | red | #ed1b32 |
| Dates, highlights | red-dark | #bf1e29 |
| Links (underlined) | teal | #3d8aa7 |
| Testimonials | ink-quote | #202124 |

**Contrast note:** Grey on grey-pale is 4.3:1 (kept exact). Avoid small text on grey-pale.

### Typography (on 720px canvas; scale by width / 720)
- **Cover:** company 40px bold, title 20px bold, date 20px
- **Content:** slide title 26px bold, body 11px, quote 9px italic
- **Labels:** confidential 6px (Raleway), slide number 10px (Lato)
- All fonts from Google Fonts

### Layout
- 16:9 canvas, 720 × 405px in source
- Top strip height: 38px
- Slide margins: 57px left & right
- Title top: 104px from edge
- Body top: 164px from edge
- No shadows, gradients, borders, or rounded corners
- All text top-left aligned

### Logos
- **Mark:** Multi-colour, cannot be recolored
  - Cover: top-right, 34px wide
  - Content: above title, 52px wide
  - Only on white or grey-pale backgrounds
- **Full logo:** Place on white or grey-pale only; wordmark disappears on red-dark
- **Google badge:** Testimonials only, 212px wide, genuine reviews only

## Sharing the Brand

Pass this link to anyone building Channel Digital materials:
**https://claude.ai/code/artifact/02e5b43d-262a-4e61-abf6-697e47513f47**

Point to the **channel-digital-design-system** project for assets, detailed specs, and design tokens.

## Updating the Brand

When Channel Digital updates its brand:
1. Update files in **channel-digital-design-system**
2. Commit and push
3. All projects should re-sync

---

**Last updated:** 2026-10-08  
**Source:** Channel Proposal Template 2026 + Channel Digital Brand Guidelines
