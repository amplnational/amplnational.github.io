---
name: AMPL
description: Association of Muslims in Politics and Law, set as an amended bill in California legislative print.
colors:
  bond-paper: "#fdfdfb"
  ink: "#121214"
  ink-secondary: "#47474d"
  ink-tertiary: "#6b6b72"
  insertion-blue: "#1a3cc8"
  on-blue: "#ffffff"
  on-blue-secondary: "#d9e0ff"
  deletion-red: "#c4211a"
  field-stroke: "#c9c9cf"
  map-wash: "#eef1fb"
  roll-highlight: "#e7ecff"
typography:
  display:
    fontFamily: "Public Sans, system-ui, sans-serif"
    fontSize: "clamp(2rem, min(5.6vw, 8.6vh), 5.25rem)"
    fontWeight: 900
    lineHeight: 1
    letterSpacing: "-0.035em"
  headline:
    fontFamily: "Public Sans, system-ui, sans-serif"
    fontSize: "clamp(1.9rem, 3.6vw, 3.1rem)"
    fontWeight: 800
    lineHeight: 1.05
    letterSpacing: "-0.03em"
  title:
    fontFamily: "Public Sans, system-ui, sans-serif"
    fontSize: "clamp(1.5rem, 2.6vw, 2.2rem)"
    fontWeight: 800
    lineHeight: 1.1
    letterSpacing: "-0.02em"
  amendment:
    fontFamily: "Tinos, Times New Roman, serif"
    fontSize: "clamp(1.35rem, 2.4vw, 1.8rem)"
    fontWeight: 400
    lineHeight: 1.35
  body:
    fontFamily: "Tinos, Times New Roman, serif"
    fontSize: "1.125rem"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "Public Sans, system-ui, sans-serif"
    fontSize: "0.95rem"
    fontWeight: 600
    lineHeight: 1.3
  enumerator:
    fontFamily: "Tinos, Times New Roman, serif"
    fontSize: "1.3rem"
    fontWeight: 700
  line-number:
    fontFamily: "Tinos, Times New Roman, serif"
    fontSize: "0.8rem"
    fontWeight: 400
    lineHeight: 2
rounded:
  none: "0px"
spacing:
  line: "2rem"
  margin: "4.5rem"
  gutter: "clamp(1.25rem, 4vw, 4rem)"
  section-top: "clamp(4rem, 9vw, 7.5rem)"
  section-bottom: "clamp(3rem, 6vw, 5rem)"
components:
  button-primary:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.bond-paper}"
    typography: "{typography.label}"
    rounded: "{rounded.none}"
    padding: "0.85rem 1.1rem"
  button-primary-hover:
    backgroundColor: "{colors.insertion-blue}"
    textColor: "{colors.bond-paper}"
  button-light:
    backgroundColor: "{colors.on-blue}"
    textColor: "{colors.insertion-blue}"
    rounded: "{rounded.none}"
    padding: "0.85rem 1.1rem"
  button-light-hover:
    backgroundColor: "{colors.on-blue-secondary}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.none}"
    padding: "0.85rem 1.1rem"
  button-ghost-hover:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.bond-paper}"
  input-field:
    backgroundColor: "{colors.on-blue}"
    textColor: "{colors.ink}"
    rounded: "{rounded.none}"
    padding: "0.85rem 0.9rem"
  select-campus:
    backgroundColor: "{colors.on-blue}"
    textColor: "{colors.ink}"
    rounded: "{rounded.none}"
    padding: "0.95rem 2.75rem 0.95rem 1rem"
  status-tag:
    backgroundColor: "{colors.on-blue}"
    textColor: "{colors.insertion-blue}"
    rounded: "{rounded.none}"
    padding: "0.25rem 0.55rem"
---

# Design System: AMPL

## Overview

**Creative North Star: "The Amended Bill"**

The public site is printed like a California legislative bill: white bond paper, black ink, a line-numbered left margin, numbered sections (SEC. 1., SEC. 2.), lettered subsections ((a), (b)) and enumerated paragraphs ((1), (2)). Amendment is the voice. Struck red text names the status quo AMPL changes; bold blue italic insertions name what it builds. The bill's structure is the composition, never decoration laid over a generic page.

Insertion blue is a field, not a trim color. It owns whole full-bleed bands (the digest under the headline, the Get Involved motions section, the footer's enacting clause) and inverts everything inside them. Outside those bands the page is ink on paper with blue reserved for enumerators, section numbers, links and active states. Density is generous and readable: statute body text at 1.125rem Tinos, set against heavy Public Sans headings in the voice of civic signage.

This system replaces the earlier navy, gold and cream serif editorial look entirely. The rejected references are the "law nonprofit" navy-gold template and the broadsheet-editorial look.

**Key Characteristics:**
- Bond paper, black ink, one insertion blue that owns full-width bands, deletion red only on strikes.
- Public Sans for headings, labels and controls; Tinos for statute text, insertions, enumerators and line numbers.
- Line-numbered left margin running the full height of the page.
- Hard rectangular edges everywhere; no radius, no elevation.
- One amendment animation per section; nothing else moves.

## Colors

A three-ink print palette: paper and black for the statute, one saturated insertion blue for fields and marks, a red that exists only to strike.

### Primary
- **Insertion Blue** (`insertion-blue`): the system's single voice. Full-bleed band backgrounds (digest, motions section, footer), the 6px rule along the top of the sticky masthead, section numbers, enumerators, inline links, active nav underline, focus outlines, text selection and caret. Inserted (`<ins>`) text is set in it.

### Secondary
- **Deletion Red** (`deletion-red`): struck (`<del>`) text and its strike, plus invalid-field borders and form error text. Never a fill, never a button, never decoration.

### Neutral
- **Bond Paper** (`bond-paper`): page background and masthead; the ground of the bill.
- **Ink** (`ink`): headings, body text, primary button fill.
- **Ink Secondary** (`ink-secondary`): ledes, roles, captions, meta strip, secondary nav link.
- **Ink Tertiary** (`ink-tertiary`): placeholders and scrollbar thumb.
- **On Blue** (`on-blue`): text, light buttons, select and tags set on blue fields.
- **On Blue Secondary** (`on-blue-secondary`): secondary copy, enumerators, struck text and line numbers inside blue fields; hover fill for light buttons.
- **Field Stroke** (`field-stroke`): the 2px resting border of form inputs.
- **Map Wash** (`map-wash`): the pale blue ground behind the California chapter map.
- **Roll Highlight** (`roll-highlight`): the selected chapter row in the chapter roll.

### Named Rules
**The Blue Owns Bands Rule.** Insertion blue appears either as a full-bleed field that inverts its contents, or as small marks (numbers, links, insertions, focus). It is never a tinted card, a gradient or a partial panel.

**The Red Only Strikes Rule.** Deletion red is reserved for struck text and validation errors. If red appears anywhere else, it is wrong. Inside blue fields, strikes turn on-blue-secondary instead of red.

## Typography

**Display Font:** Public Sans (with system-ui, sans-serif)
**Body Font:** Tinos (with Times New Roman, serif)

**Character:** Public Sans at weight 800 to 900 with tight negative tracking is the civic sign; Tinos is the bill's own Times, carrying the statute text, the insertions and every enumerator. The two never swap jobs.

### Hierarchy
- **Display** (900, clamp(2rem, min(5.6vw, 8.6vh), 5.25rem), line-height 1, tracking -0.035em, balanced): the amended headline in the first viewport only. Its insertion drops to Tinos bold italic 700.
- **Headline** (800, clamp(1.9rem, 3.6vw, 3.1rem), 1.05): section titles, prefixed by a 900-weight "SEC. n." in insertion blue.
- **Title** (800, clamp(1.5rem, 2.6vw, 2.2rem), 1.1): program names, speaker names, motion titles. Band and chapter-roll titles step down to 1.2 to 1.6rem at the same weight.
- **Amendment** (Tinos 400, clamp(1.35rem, 2.4vw, 1.8rem), 1.35): the one amended lede beneath each section title. Plain ledes use 1.3rem in ink-secondary, max 46ch.
- **Body** (Tinos 400, 1.125rem, 1.6): statute text; program paragraphs step to 1.2rem. Measure 40 to 60ch.
- **Label** (Public Sans 600 to 700, 0.95 to 1.05rem): nav, buttons, field labels, links in result blocks, meta strip.
- **Enumerator** (Tinos 700, 1.3 to 1.6rem, insertion blue): (a), (1), and the chapter roll's counter, in a fixed 2.5 to 3.5rem left column.
- **Line number** (Tinos 400, 0.8rem, tabular, ink at 50%): the margin numerals, every fifth line labelled, on the 2rem line grid.

### Named Rules
**The Statute Voice Rule.** Running text, insertions, enumerators and line numbers are Tinos; anything a person reads as a heading, label or control is Public Sans. Insertions are always Tinos italic bold in blue.

**The One Amendment Rule.** Each section carries exactly one amended line (a `del` and/or `ins` pair). Amendment is the voice of a key line, not a styling for emphasis elsewhere.

## Layout

A single column of sections on the line-numbered bill. Every content block sits inside a left padding of gutter plus margin (`spacing.gutter` + `spacing.margin`); the margin column holds the line numbers, generated in JS on the 2rem `spacing.line` grid and labelled every fifth line. Blue bands run full-bleed while their content keeps the same left edge, and the margin numerals inside them turn on-blue-secondary.

Sections use `section-top` / `section-bottom` padding with a 62rem max-width header block. Content inside sections is grid-based: two-column digest and picker (1.1fr / 1fr), program rows of enumerator / text / photo (3.5rem / 1fr / clamp(16rem, 32vw, 28rem)), two-column enumerated lists for speakers and motions, map plus roll for chapters, and form plus aside for contact. Column gaps scale with clamp(1.5rem to 6rem).

Breakpoints: at 960px the margin narrows to 2.4rem, every two-column grid stacks, the picker moves above the digest copy and the first-viewport photo moves below the band. At 860px the nav collapses into a Menu button dropdown. At 560px the margin is 1.9rem, the gutter 1rem, and the form goes to one column.

## Elevation & Depth

Flat. Depth comes from the blue fields, not from shadows: a surface is either paper or blue, and the line between them is a full-bleed color change. There are no drop shadows, gradients or layered cards. The ghost button's outline is drawn as an inset 2px stroke, which is a border technique and not elevation. The photo viewer dims the page with a near-opaque navy-black backdrop (rgba(10, 14, 32, 0.92)).

### Named Rules
**The Paper Or Blue Rule.** Surfaces are flat at rest and in every state. Separate regions with a blue field, a section number or space, never with a shadow or a tinted card.

## Shapes

Hard rectangles throughout (`rounded.none`): buttons, selects, inputs, tags, photos and bands are square-cornered. The only round forms belong to the AMPL mark (the crescent and the scales' finial). Photos are cropped to 4:3 (programs, record grid), 1:1 (first-viewport photo) or 3:2 (mobile first-viewport photo). Brackets are the button's silhouette: a Tinos "[" and "]" frame each action label.

The system has no decorative divider rules. Structure is carried by section numbers, margin numerals and blue fields. The lines it does draw are functional: the strike through deleted text, the 6px blue masthead rule, the 3px active-nav underline, and 2px field strokes.

## Components

### Buttons
Bracketed statute actions: hard-edged, heavy and plain.
- **Shape:** square corners (0px), Public Sans 700 at 1rem, 0.85rem by 1.1rem padding, label framed by Tinos brackets at 70% opacity.
- **Primary:** ink fill, paper text; hover turns the fill insertion blue (0.2s) while the brackets step out 3px each way (cubic-bezier(0.16, 1, 0.3, 1)).
- **Light (on blue):** white fill, blue text; hover goes on-blue-secondary.
- **Ghost:** transparent with a 2px inset ink stroke; hover fills ink. On blue fields the stroke and text are white, and the hover fill is white with blue text.
- **Disabled / sending:** 60% opacity with a progress cursor.
- **Focus:** 3px solid blue outline at a 3px offset; white inside blue fields.

### Status Tag
- **Style:** Public Sans 800 at 0.8rem, uppercase, 0.08em tracking, blue on white, square. Used only to state a real program status (Mentorship "Pending") inline after a title on blue.

### Inputs / Fields
- **Style:** white fill, 2px field-stroke border, square, Tinos 1.05rem input text; selects use Public Sans with a drawn chevron. Labels are Public Sans 700 above the field, with hints in ink-secondary.
- **Focus:** border turns insertion blue, plus a 3px blue outline on keyboard focus.
- **Error:** border turns deletion red (`:user-invalid`); the status line reports errors in red and success in blue.

### Campus Picker
The primary action, set inside the blue digest band: a borderless white full-width select (Public Sans 600, 1.05rem) under a 1.35rem Public Sans 800 label, with an `aria-live` result block below it showing the chapter name, city and links in white.

### Navigation
- **Style:** sticky paper masthead with a 6px insertion-blue top rule. Wordmark is Public Sans 900 with the full name in Tinos beside it. Links are Public Sans 600 at 0.95rem; "Chapter login" sits last at weight 400 in ink-secondary.
- **States:** hover turns links blue; the current section is blue with a 3px underline at a 0.45em offset (`aria-current`).
- **Mobile (860px and below):** a "Menu" button with a three-line icon opens a full-width paper dropdown of 1.1rem links.

### Enumerated Lists
Speakers, motions and the chapter roll share one grammar: a fixed narrow column holding a Tinos bold enumerator in blue ((1), (a)), then a Public Sans 800 title and Tinos secondary text. The selected chapter row takes the roll-highlight fill, linked to its pin on the map.

### Chapter Map
The California map image on the map-wash ground, with campus pins drawn as paper circles with a 3px blue stroke that fill blue on hover, focus or selection, joined by a dotted blue route at 55% opacity. Pin labels are Public Sans 800 at 13px with a map-wash halo.

### Amendment Motion
Each section's key line performs its amendment once when it enters view: the strike draws left to right (0.7s), then the insertion resolves from a 6px blur to sharp (0.8s, 0.6s delay), both on cubic-bezier(0.16, 1, 0.3, 1). With reduced motion or without JS the final amended text shows static. Apart from button hover and the photo hover lift, nothing else animates.

## Logo

The mark is the incumbent AMPL emblem redrawn as one-colour vector: a crescent, horns up, holding the scales of justice. The design is unchanged from `images/logo.jpg`; only the file and colouring are new.

- `images/ampl-mark.svg`: crescent and scales only. Use at 40px and below (masthead, favicon). Inline it with `fill="currentColor"` so it takes `--blue` on paper and `--on-blue` on bands.
- `images/ampl-seal.svg` / `images/ampl-seal-white.svg`: the full seal with "Association of Muslims in Politics and Law" on the ring and "National" below. Use at 96px and up (footer, social avatars, print). Ring text is live Tinos with a Times fallback; outline it in a design tool before sending it to print.
- `images/ampl-lockup.svg`: the mark beside "AMPL" in Public Sans 900.
- One colour only: insertion blue on paper, white on blue, or cream `#d8cdb6` on the legacy navy. No gradients, outlines or drop shadows.
- `images/logo.jpg` stays as the legacy raster (favicon fallback, portal.html until it migrates).

## Do's and Don'ts

### Do:
- **Do** set every surface as paper or a full-bleed insertion-blue field, and invert all content inside the field (white text, on-blue-secondary secondary text, white focus rings).
- **Do** number structure the way a bill does: "SEC. n." on section titles, (a) for subsections, (1) for enumerated items, all in Tinos bold blue except the 900-weight Public Sans section number.
- **Do** keep the line-numbered left margin and align all content to the gutter-plus-margin edge.
- **Do** give each section one amended line, with insertions in Tinos bold italic blue and deletions struck in red (on-blue-secondary inside blue fields).
- **Do** keep every control square-cornered, and frame button labels with Tinos brackets.

### Don't:
- **Don't** use rounded corners, drop shadows, gradients or tinted cards; depth is paper versus blue.
- **Don't** use deletion red for anything except struck text and validation errors.
- **Don't** separate sections with divider rules; use section numbers, margin numerals and blue fields.
- **Don't** return to the navy, gold and cream serif palette or the broadsheet-editorial layout this system replaced.
- **Don't** animate anything beyond the one amendment per section and the small hover responses.

## Not yet migrated

`portal.html` (the private Chapter Portal) still uses the previous navy and cream style and was out of scope for this redesign. Its tokens are not part of this system; when it is migrated it should adopt the tokens above.
