# Channel Digital Brand Guidelines

Channel Digital is a web design, hosting and SEO agency in Truro, Cornwall. These guidelines cover all proposal and quote decks, and are extensible to presentations and new designs.

## Content Fundamentals

- Write in the first person plural for the agency and address the client as "you": "Let us know if you'd like to chat further."
- Keep the tone plain and warm. The closing line is "I look forward to hearing from you."
- Set the client's company name, the proposal title and the date on the cover in capitals. Set every other title in title case or sentence case: "Project Overview", "Next Steps", "What our clients say".
- Use British spelling. No emoji.
- Sign off with a name, a job title, then labelled contact lines: bold "E:", "P:", "M:" followed by the value.
- Quote testimonials in full, in curly double quotes, followed by the person's name and their company in brackets.

## Colour

All values are defined in `tokens.json`.

- **Slides are `white`.** Text is `grey`. Do not use black.
- **`red-dark`** is for the date on the cover.
- **`red`** belongs to the logo mark; use it for shapes or for large bold text only, never for small text.
- **`teal`** is for links, and links are always underlined.
- **`grey-pale`** is the strip across the top of every content slide and the fill behind the cover image.
- **`teal-light` and `grey-light`** are logo colours. Use them for shapes, never for text.
- **Testimonials** are set in `ink-quote`, not `grey`.

### Contrast Requirements

Two pairs in the source miss 4.5:1 for small text and are kept exact:
- `teal` links on `white` (3.9:1)
- `grey` on `grey-pale` (4.3:1)

**Do not put small text on `grey-pale`.** All other combinations meet WCAG AA.

## Typography

All fonts are loaded from Google Fonts; no font files are stored locally.

- **Open Sans** carries everything: titles in bold, body in regular.
- **Raleway** appears once, for the "Confidential" label on the cover.
- **Lato** appears once, for the slide number.

### Type Scales

See `tokens.json` for all type definitions. Key styles:

- **Titles:** `slide-title`, bold, `grey`, left aligned
- **Body:** `body`, line height 1.15, `grey`, left aligned, with no bullets
- **Testimonials:** `quote` (italic) with `attribution` (bold) beneath

### Note on Size

The text is small because the deck is a proposal read on a screen or as a PDF. **It is too small to present in a room.** For presentations, enlarge all type proportionally.

## Layout

- **Canvas:** 16:9 (720 x 405px in source; scale to other sizes by multiplying by `canvas-width / 720`)
- **Corners:** Square everywhere (`radius-none`). No shadows, no gradients, no borders.
- **Top Strip:** Every slide has a strip across the top, `strip-height` tall
  - Cover: `white` background
  - Content slides: `grey-pale` background
- **Margins:** Title and body share left and right margins of `slide-margin` (57px on the 720px canvas)
- **Text Alignment:** Top-left aligned everywhere. Nothing is centred.

### Slide Layouts

**Cover Slide:**
- Top strip in `white` containing logo mark (top right) and "Confidential" label (top left)
- Client's company name below (capitals, `grey`)
- Proposal title below that (capitals, `grey`)
- Date below that (`red-dark`)
- Pale geometric background (Backgrounds group) from 36px below strip to bottom
- Background fill under geometry: `grey-pale`

**Content Slide:**
- Top strip in `grey-pale` containing logo mark (top right)
- Title starts at `title-top` (104px from slide top)
- Body starts at `body-top` (164px from slide top)
- No imagery other than logo mark

**Testimonial Slide:**
- Two-column layout: title and Google badge on left, quotes on right from 51% of width
- Google five-star badge (212px wide on 720px canvas) below title in left column

## Imagery

- The cover carries a pale geometric background (see `assets/backgrounds/`) below the top strip.
- Content slides carry no imagery other than the logo mark.
- The source file holds five photographs in layouts no slide currently uses. They are not in this system because their licensing is not recorded.

## Logo and Iconography

### Logo Mark

**File:** `channel-logo-mark.png` (840 x 596, transparent)

- Slides carry the logo mark alone, as the agency's own deck does
- Top right of the cover strip: 34px wide on 720px canvas
- Above the title on content slides: 52px wide on 720px canvas
- Multi-colour and cannot be recoloured
- Place it on `white` or `grey-pale` only. Never on `red-dark`.

### Full Logo

**File:** `channel-digital-logo.png` (1326 x 468, transparent)

The full logo is the mark with the "channel DIGITAL" wordmark to its right.

- Use where the name must appear with the mark
- The wordmark was enlarged from the live website (slightly soft edges); do not show it wider than about 660px on a 1920px slide
- **Replace it when the agency supplies a vector logo**
- Place it on `white` or `grey-pale`; the wordmark is dark grey and disappears on `red-dark`
- Do not redraw, recolour, or crop the logo, and never set the wordmark in another typeface

### Other Graphics

- **Google Five-Star Badge:** Used on testimonial slide only, 212px wide on 720px canvas. Carries Google's logo; do not alter it.
- No icon set is used. No other graphics appear in the system.

## Scaling for Different Canvas Sizes

All measurements in these guidelines are in pixels on a 720 x 405 canvas, where 1px equals 1pt in the source deck.

**For other canvas sizes, multiply by: `canvas-width / 720`**

Example: On 1920 x 1080, multiply by 2.667
- `slide-title` at 26px becomes 69px
- Logo mark at 52px becomes 139px
- `slide-margin` at 57px becomes 152px

## File Organization

Use the structure in the design system project:

```
assets/
  logos/
    channel-logo-mark.png
    channel-digital-logo.png
  backgrounds/
    cover-background-geometric.png
  badges/
    google-five-star-badge.png
```

## Questions & Updates

If the agency updates its brand, brand materials, or logo:
1. Update the relevant assets in `assets/`
2. Update this BRAND.md and `tokens.json`
3. Notify all projects to resync

For questions about applying this system, refer to `docs/implementation/`.
