---
name: AMPL
description: Association of Muslims in Politics and Law. A sober, institutional student network set beside the bar associations.
colors:
  navy: "#1c2541"
  navy-hover: "#27315a"
  navy-deep: "#141b31"
  link-navy: "#2d3c74"
  silver: "#c3c8d2"
  page-gray: "#edeff3"
  surface: "#f6f7f9"
  panel: "#fbfbfc"
  field-white: "#ffffff"
  ink: "#1a2133"
  ink-secondary: "#485064"
  ink-tertiary: "#5f6678"
  hairline: "#d3d7df"
  hairline-soft: "#e2e5ea"
  on-navy: "#ffffff"
  on-navy-secondary: "#b8c0d4"
  error-red: "#a8322b"
  success-green: "#2c6e49"
  warning-amber: "#8a5a12"
typography:
  display:
    fontFamily: "Source Serif 4, Georgia, Times New Roman, serif"
    fontSize: "clamp(2.15rem, 4vw, 3.25rem)"
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: "-0.015em"
  headline:
    fontFamily: "Source Serif 4, Georgia, Times New Roman, serif"
    fontSize: "clamp(1.75rem, 3vw, 2.4rem)"
    fontWeight: 600
    lineHeight: 1.15
    letterSpacing: "-0.01em"
  title:
    fontFamily: "Source Serif 4, Georgia, Times New Roman, serif"
    fontSize: "1.3rem"
    fontWeight: 600
    lineHeight: 1.3
  quote:
    fontFamily: "Source Serif 4, Georgia, Times New Roman, serif"
    fontSize: "clamp(1.5rem, 2.8vw, 2.1rem)"
    fontWeight: 500
    lineHeight: 1.3
  wordmark:
    fontFamily: "Source Serif 4, Georgia, Times New Roman, serif"
    fontSize: "1.3rem"
    fontWeight: 600
    letterSpacing: "0.04em"
  lede:
    fontFamily: "Public Sans, system-ui, -apple-system, Segoe UI, sans-serif"
    fontSize: "1.2rem"
    fontWeight: 400
    lineHeight: 1.6
  body:
    fontFamily: "Public Sans, system-ui, -apple-system, Segoe UI, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 400
    lineHeight: 1.65
  label:
    fontFamily: "Public Sans, system-ui, -apple-system, Segoe UI, sans-serif"
    fontSize: "0.94rem"
    fontWeight: 600
    lineHeight: 1.2
  tag:
    fontFamily: "Public Sans, system-ui, -apple-system, Segoe UI, sans-serif"
    fontSize: "0.72rem"
    fontWeight: 600
    lineHeight: 1
    letterSpacing: "0.06em"
rounded:
  tag: "2px"
  base: "3px"
spacing:
  wrap: "72rem"
  gutter: "clamp(1.25rem, 4vw, 2.5rem)"
  section: "clamp(4rem, 8vw, 6rem)"
  section-head: "clamp(2.25rem, 4vw, 3rem)"
  hero-top: "clamp(2.75rem, 5.5vw, 4.25rem)"
  hero-bottom: "clamp(3rem, 6vw, 4.5rem)"
  column-gap: "clamp(2rem, 5vw, 4rem)"
components:
  button-primary:
    backgroundColor: "{colors.navy}"
    textColor: "{colors.on-navy}"
    typography: "{typography.label}"
    rounded: "{rounded.base}"
    padding: "0.8rem 1.2rem"
  button-primary-hover:
    backgroundColor: "{colors.navy-hover}"
    textColor: "{colors.on-navy}"
  button-outline:
    backgroundColor: "transparent"
    textColor: "{colors.navy}"
    typography: "{typography.label}"
    rounded: "{rounded.base}"
    padding: "0.8rem 1.2rem"
  button-outline-hover:
    backgroundColor: "rgba(28, 37, 65, 0.04)"
    textColor: "{colors.navy}"
  button-on-navy:
    backgroundColor: "transparent"
    textColor: "{colors.on-navy}"
    rounded: "{rounded.base}"
    padding: "0.45rem 0.9rem"
  button-on-navy-hover:
    backgroundColor: "rgba(255, 255, 255, 0.08)"
    textColor: "{colors.on-navy}"
  input-field:
    backgroundColor: "{colors.field-white}"
    textColor: "{colors.ink}"
    rounded: "{rounded.base}"
    padding: "0.75rem 0.85rem"
  picker-panel:
    backgroundColor: "{colors.panel}"
    textColor: "{colors.ink}"
    rounded: "{rounded.base}"
    padding: "1.4rem 1.5rem 1.25rem"
  panel-card:
    backgroundColor: "{colors.panel}"
    textColor: "{colors.ink}"
    rounded: "{rounded.base}"
    padding: "1.25rem 1.5rem"
  status-tag:
    backgroundColor: "{colors.panel}"
    textColor: "{colors.ink-secondary}"
    typography: "{typography.tag}"
    rounded: "{rounded.tag}"
    padding: "0.3rem 0.45rem"
  nav-link:
    textColor: "{colors.on-navy-secondary}"
    typography: "{typography.label}"
  nav-link-active:
    textColor: "{colors.on-navy}"
---

# Design System: AMPL

## Overview

**Creative North Star: "The Bar Association Standard"**

AMPL sits on the same shelf as the Muslim Bar Association, NAPABA and the American Constitution Society, and looks like it belongs there. The system is the category standard played straight: a muted cool-gray page, deep AMPL navy owning the header, the hero and the footer, a serif for headings and a plain civic sans for everything a person reads or operates. There is no conceit and no ornament. Credibility comes from restraint, clear hierarchy and real photographs of members.

Density is calm and readable. Content sits in a 72rem column, sections breathe on generous vertical padding, and structure is drawn with 1px hairlines and quiet tonal steps between the page gray, a lighter alternate band and near-white panels. Navy is reserved for the institutional frame (top and bottom of the page, plus the hero) and for primary actions, links and the active state.

This world replaces the earlier "Amended Bill" system entirely, and the navy, gold and cream serif template before it. Both are rejected.

**Key Characteristics:**
- Muted cool-gray page, never stark white; a slightly lighter band alternates sections.
- Deep navy header, hero and footer, with the AMPL mark in silver.
- Source Serif 4 at 600 for headings; Public Sans for body, labels and controls.
- Gently squared corners (3px), 1px hairlines, no shadows, no gradients.
- Motion is near-silent: a 4px rise, a 3% photo scale, a 2px arrow nudge.

## Colors

A restrained institutional palette: one deep navy, a family of cool grays, silver for the mark, and status colors used only for status.

### Primary
- **AMPL Navy** (`navy`): the masthead, the hero band, primary button fills, the active portal tab, map pins when selected, pillar top rules, text selection. Hover on navy fills steps to **Navy Hover** (`navy-hover`).
- **Navy Deep** (`navy-deep`): the footer only, one step darker so the page closes firmly.
- **Link Navy** (`link-navy`): inline links, the focus outline on light grounds, the success status line. Slightly lifted from navy so links read as links against ink.

### Secondary
- **Silver** (`silver`): the AMPL mark on navy, the footer seal, and the 2px active-nav underline. Nothing else.

### Neutral
- **Page Gray** (`page-gray`): the body ground. **Surface** (`surface`): alternate section bands, the chapter strip, the map ground, the portal sidebar. **Panel** (`panel`): cards, the picker, the contact form, the call-to-action row. **Field White** (`field-white`): input and select fills only.
- **Ink** (`ink`), **Ink Secondary** (`ink-secondary`), **Ink Tertiary** (`ink-tertiary`): headings and body, ledes and supporting copy, hints, placeholders and empty states.
- **Hairline** (`hairline`): every border and divider. **Hairline Soft** (`hairline-soft`): row dividers inside portal cards, the selected chapter row, photo placeholders.
- **On Navy** / **On Navy Secondary** (`on-navy`, `on-navy-secondary`): headings and lede text inside navy bands, nav links at rest; on-navy hairlines are white at 14% opacity.
- **Error Red** (`error-red`): validation errors and destructive portal actions. **Success Green** (`success-green`) and **Warning Amber** (`warning-amber`): portal status badges and approve actions only.

### Named Rules
**The Navy Frame Rule.** Navy owns the header, the hero and the footer as full-width bands, and otherwise appears only as small marks: primary buttons, links, the active tab, selected pins. Never a navy card or a navy section in the middle of the page.

**The No Stark White Rule.** The page is page gray and alternate bands are surface. Pure white is for form fields; panels are the near-white panel tone.

## Typography

**Display Font:** Source Serif 4 (with Georgia, Times New Roman, serif)
**Body Font:** Public Sans (with system-ui, -apple-system, Segoe UI, sans-serif)

**Character:** A sober text serif at semibold for anything that names a thing, set against a neutral government-grade sans for reading and operating. The pairing reads as legal publishing, not as a campaign.

### Hierarchy
- **Display** (600, clamp(2.15rem, 4vw, 3.25rem), 1.1, tracking -0.015em, balanced): the hero headline only, white on navy.
- **Headline** (600, clamp(1.75rem, 3vw, 2.4rem), 1.15): section titles. Portal page titles use 1.85rem.
- **Title** (600, 1.3rem, 1.3): program names, ways to get involved; speaker names at 1.25rem; portal card titles at 1.2rem.
- **Quote** (Source Serif 4, clamp(1.5rem, 2.8vw, 2.1rem), 1.3, max 44rem): the single pull quote in About.
- **Wordmark** (600, 1.3rem, tracking 0.04em): "AMPL" beside the mark, with the full name below in Public Sans 0.78rem on-navy-secondary.
- **Lede** (Public Sans 400, 1.2rem, 1.6, max 40rem): one line or short paragraph under each section title, ink-secondary; 1.15rem on-navy-secondary in the hero.
- **Body** (Public Sans 400, 1.0625rem, 1.65; 1rem under 600px): running text, measure held near 30 to 40rem. The portal runs denser at 0.97rem, 1.55.
- **Label** (Public Sans 600, 0.92 to 0.97rem): buttons, field labels, nav (500 at rest), roll links, result links.
- **Tag** (Public Sans 600, 0.72rem, uppercase, 0.06em tracking): status tags only.

### Named Rules
**The Serif Names, Sans Works Rule.** Source Serif 4 is for headings, names, the wordmark and the one pull quote; everything read at length or clicked is Public Sans. Serif headings stay at 600; they are never light, never italic, never uppercase.

## Layout

A centered 72rem column (`spacing.wrap`) with a fluid gutter (`spacing.gutter`), stacked as full-width bands: navy masthead (sticky, 4.5rem tall), navy hero, a surface-colored chapter strip at the fold, then sections alternating page gray and surface (the alternate band adds a hairline top and bottom), ending in the navy-deep footer.

Sections use `spacing.section` vertical padding with a `spacing.section-head` gap below the title block. Inside sections the grids are simple: hero at 1.15fr / 1fr (copy and picker left, photo right); three equal pillars; programs at 0.8fr / 1.2fr with a sticky heading; a four-up gallery and four-up speaker list; map beside chapter roll; two ways to get involved split by a vertical hairline; contact form at 1.5fr beside a 1fr details column. Column gaps follow `spacing.column-gap`.

Breakpoints: at 1080px the nav tightens and the name under the wordmark hides. At 960px the nav collapses into a Menu button with a full-width navy dropdown, every two-column grid stacks, pillars go to one column, and the gallery and speakers go two-up. At 600px body text drops to 1rem, the hero photo moves below the picker, speakers and the form go to one column, and CTA buttons go full width. The portal is a 240px sidebar beside content up to 1100px, collapsing at 900px into a horizontal tab strip.

## Elevation & Depth

Flat. Depth is tonal: page gray, a lighter surface band, a near-white panel with a 1px hairline, and navy for the frame. There are no drop shadows and no gradients. The active nav underline and the portal's active auth tab are drawn as an inset 2px box-shadow, which is a line technique, not elevation. The photo viewer dims the page with a navy-black backdrop (rgba(14, 19, 34, 0.92)).

### Named Rules
**The Hairline Not Shadow Rule.** Separate regions with a tonal step or a 1px hairline. If a panel needs to lift, it gets the panel tone and a border, never a shadow.

## Shapes

Gently squared: every control, panel, photo and card takes a 3px radius (`rounded.base`); status tags and badges take 2px (`rounded.tag`). Lines are 1px hairlines throughout; the only heavier lines are the 1px navy rule over each pillar and the 2px silver active-nav underline. Photos crop to 4:3 (hero and gallery). The only round forms belong to the AMPL mark and the map pins.

## Components

### Buttons
Plain, solid and quiet.
- **Shape:** 3px corners, 1px border, Public Sans 600 at 0.97rem, 0.8rem by 1.2rem padding. An optional 15px trailing arrow nudges 2px right on hover.
- **Primary:** navy fill and border, white text; hover steps to navy hover (0.15s).
- **Outline:** transparent, navy text, a gray border (#a4abba); hover turns the border navy over a 4% navy wash.
- **On navy:** the Chapter login and Menu buttons: transparent, white text, a white border at 35%; hover adds an 8% white wash.
- **Portal variants:** a light button (panel fill, hairline border, navy text), a small size (0.35rem by 0.75rem, 0.84rem), and success-green and error-red fills for approve and deny.
- **Disabled / sending:** 55 to 60% opacity.
- **Focus:** 2px link-navy outline at a 3px offset; white inside navy bands.

### Status Tag
- **Style:** uppercase Public Sans 600 at 0.72rem, 0.06em tracking, ink-secondary on panel with a hairline border, 2px corners, set inline after a title. Used only to state a real status ("Coming soon").
- **Portal badges:** the same shape in sentence case, colored by state with a 1px currentColor border on a pale tint: amber pending, green approved or income, red denied or expense, navy admin.

### Cards / Containers
- **Corner Style:** 3px.
- **Background:** panel on page gray or surface.
- **Shadow Strategy:** none (see Elevation & Depth).
- **Border:** 1px hairline.
- **Internal Padding:** 1.25 to 2rem; the contact form scales with clamp(1.25rem, 3vw, 2rem), portal cards use 1.6rem.

### Inputs / Fields
- **Style:** white fill, 1px hairline border, 3px corners, Public Sans 1rem, 0.75rem by 0.85rem padding; selects draw a 12px chevron at the right. Labels sit above in Public Sans 600, hints in ink-tertiary.
- **Hover / Focus:** border darkens to #aab0bd on hover and turns navy on focus, plus a 2px link-navy outline at a 2px offset for keyboard focus.
- **Error:** border turns error red on `:user-invalid`; the status line reports errors in error red and success in link navy.

### Navigation
- **Style:** sticky navy masthead with a white 14% hairline below. The 38px silver mark leads the serif wordmark. Links are Public Sans 500 at 0.94rem in on-navy-secondary; "Chapter login" sits last as an on-navy outline button.
- **States:** hover and the current section turn white; the current section adds a 2px silver underline (`aria-current`).
- **Mobile (960px and below):** a bordered Menu button opens a full-width navy dropdown of 1.05rem links divided by on-navy hairlines, with Chapter login centered at the bottom.
- **Portal:** a fixed 64px navy bar with a 32px silver mark; sidebar tabs fill navy when active and hairline-soft on hover.

### Campus Picker
The primary action, a panel set inside the navy hero: a bold "Find your chapter" label over a full-width white select, with an `aria-live` result block below showing the chapter name, city and links. Each new result rises 4px into place over 0.35s; reduced motion removes it.

### Chapter Map and Roll
The California map on the surface ground inside a hairline frame, with pins drawn as panel circles with a 2.5px navy stroke that fill navy on hover, focus or selection; labels are Public Sans 600 at 13px with a surface halo. The roll beside it lists school, city and links between hairlines; the selected row takes a hairline-soft fill.

### Photo Gallery
Four-up 4:3 photos with 3px corners and a short caption below in ink-secondary; hover scales the image 3% over 0.5s, and a click opens the photo viewer.

## Logo

The mark is the incumbent AMPL emblem redrawn as one-colour vector: a crescent, horns up, holding the scales of justice. The SVG files in `images/` are unchanged by this redesign.

- `images/ampl-mark.svg`: crescent and scales only. Use at 40px and below (masthead, portal bar, favicon). Inline it with `fill="currentColor"` so it takes the color of its context; both index.html and portal.html inline it.
- `images/ampl-seal.svg` (navy) / `images/ampl-seal-silver.svg`: the full seal with "Association of Muslims in Politics and Law" on the ring and "National" below. Use at 96px and up (footer, social avatars, print). The ring text is live text in the file; outline it in a design tool before sending it to print.
- `images/ampl-lockup.svg`: the mark beside "AMPL".
- One colour only. On the public site the mark renders silver (`#c3c8d2`) on navy, and the footer uses `images/ampl-seal-silver.svg` at 104px. No gradients, outlines or drop shadows.
- `images/logo.jpg` stays as the legacy raster favicon fallback.

## Do's and Don'ts

### Do:
- **Do** keep the page muted: page gray ground, surface for alternate bands, panel for cards, white only inside form fields.
- **Do** frame every page in navy: navy header and hero, navy-deep footer, silver mark.
- **Do** set headings, names and the wordmark in Source Serif 4 at 600, and everything else in Public Sans.
- **Do** use 3px corners and 1px hairlines on every control, panel and photo.
- **Do** make the primary action a navy-filled button and secondary actions outline buttons.
- **Do** keep motion to the 4px picker rise, the 3% photo scale and the 2px arrow nudge, all on cubic-bezier(0.22, 1, 0.36, 1), and remove the rise under reduced motion.

### Don't:
- **Don't** return to the amended-bill concept: no line-numbered margin, no section numbering, no strike-and-insert amendments, no bracketed buttons. The user rejected it as too unique and playful.
- **Don't** return to the navy, gold and cream serif template; it is also rejected.
- **Don't** use a bright or stark white page, drop shadows or gradients.
- **Don't** put navy cards or navy bands in the middle of the page; navy is the frame and the primary action.
- **Don't** use silver for anything but the mark, the seal and the active-nav underline.
- **Don't** use red, green or amber outside status, validation and destructive actions.
