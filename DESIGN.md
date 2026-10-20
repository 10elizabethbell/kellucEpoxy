---
name: Kelluc Epoxy
description: Calm paper and navy bands for a Windsor-Essex epoxy floor installer, with the logo's red as the one accent.
colors:
  red: "#d42a2f"
  red-hover: "#b8232a"
  red-ink: "#b01e24"
  red-on-dark: "#ff6b6b"
  red-display: "#f2484d"
  paper: "#f4f5f8"
  card: "#ffffff"
  field: "#e7eaf0"
  ink: "#161d29"
  body: "#2b3442"
  soft: "#4e5868"
  navy: "#1f2836"
  deep: "#141a25"
  on-dark: "#f4f6fa"
  on-dark-soft: "#c4cbd8"
  line: "rgba(22,29,41,.12)"
  focus: "#2f66d0"
  error: "#b3261e"
typography:
  display:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(42px, 12vw, 80px)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-.005em"
  headline:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(30px, 7.6vw, 48px)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-.005em"
  title:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(20px, 5.4vw, 22px)"
    fontWeight: 400
    lineHeight: 1.2
  button:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(17px, 4.6vw, 19px)"
    fontWeight: 400
    lineHeight: 1.7
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.7
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "14px"
    fontWeight: 400
    lineHeight: 1
rounded:
  field: "10px"
  row: "18px"
  card: "24px"
  pill: "999px"
spacing:
  gutter-phone: "20px"
  gutter-desktop: "40px"
  section-phone: "64px"
  section-desktop: "96px"
  column-gap: "64px"
  stack: "16px"
  block: "28px"
  container: "1160px"
components:
  button-primary:
    backgroundColor: "{colors.red}"
    textColor: "{colors.card}"
    typography: "{typography.button}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.red-hover}"
    textColor: "{colors.card}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    typography: "{typography.button}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-quiet:
    backgroundColor: "{colors.card}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 20px"
    height: "48px"
  service-row:
    backgroundColor: "rgba(255,255,255,.06)"
    textColor: "{colors.on-dark}"
    typography: "{typography.title}"
    rounded: "{rounded.row}"
    padding: "12px 14px 12px 22px"
    height: "64px"
  arrow-circle:
    backgroundColor: "rgba(255,255,255,.1)"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.pill}"
    size: "44px"
  arrow-circle-hover:
    backgroundColor: "{colors.red}"
    textColor: "{colors.card}"
  form-card:
    backgroundColor: "{colors.card}"
    rounded: "{rounded.card}"
    padding: "clamp(20px, 5vw, 32px)"
  input:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.field}"
    padding: "13px 14px"
    height: "52px"
  chip:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 18px"
    height: "48px"
  chip-selected:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.card}"
  step-number:
    backgroundColor: "{colors.red}"
    textColor: "{colors.card}"
    rounded: "{rounded.pill}"
    size: "48px"
  float-messenger:
    backgroundColor: "{colors.red}"
    textColor: "{colors.card}"
    rounded: "{rounded.pill}"
    size: "60px"
---

# Design System: Kelluc Epoxy

## Overview

**Creative North Star: "The Finished Floor"**

A calm, phone-first page that reads like a well-sealed floor: smooth paper and graphite surfaces, nothing loud, one hit of the logo's red where the visitor should act. It is Ellie's house calm band style adapted to Kelluc's badge. The logo's black becomes two navies (never black itself), and the triquetra's red becomes the single accent fill.

The page is a stack of full-bleed bands alternating light and dark so each new section is obvious without dividers: a paper header, the client's own flake-finish front steps under a deep navy overlay, paper, navy, paper, deep navy with a faint diagonal line texture, paper, navy, and a textured deep-navy footer. Density is low: one idea per band, short headings in Cal Sans, generous 64px/96px band padding. Shapes are soft and borderless. Motion is limited to one hero entrance, one fade-up and the floating Messenger circle.

Every action leads to Facebook Messenger, so the red fill only marks Messenger-bound or quote actions, the numbered steps and the arrow circles on hover.

**Key Characteristics:**
- Paper / graphite navy / deep navy bands; the ground is never black.
- One accent hue (logo red) in five tuned shades, each with a set job.
- Cal Sans headings at weight 400, system-stack body at 16px / 1.7.
- Pill buttons, 24px cards, 18px rows, 10px fields; no borders on surfaces.
- Flat surfaces; the only shadow belongs to the floating Messenger circle.
- Hero H1 letter bounce-in, one 12px fade-up, everything static under reduced motion.

## Colors

Cool, quiet neutrals carry the page; the logo's red appears in small, deliberate doses.

### Primary
- **Triquetra Red** (red): the one accent fill. Primary buttons, the numbered step circles, arrow circles on hover, the floating Messenger circle, text selection. Text on it is always white (about 5:1); navy on red fails.
- **Pressed Red** (red-hover): primary button hover only. Keeps white text above 6:1.
- **Ink Red** (red-ink): red as text or icon on light grounds: the accent word in light-band headings, the "why" claim icons, header icon hover (6.3:1 on paper).
- **Signal Red** (red-on-dark): small red text and focus rings on navy, deep navy and the photo hero, and the H1 accent word over the hero photo (5.3:1 on navy).
- **Display Red** (red-display): large accent words in headings on navy and deep navy only. Closer to the logo red; 4.1:1 on navy and 4.8:1 on deep navy, so it is legal for large text only.

### Neutral
- **Paper** (paper): page ground, header, light bands, `theme-color`.
- **White Card** (card): the quote form card and the "quiet" button fill.
- **Field Grey** (field): inputs, chips and the copy-message panel on the white card. About 1.2:1 against the card; fields are identified by their labels and fill, and keyboard/hover state comes from the focus blue.
- **Ink** (ink): headings and labels on light; the selected-chip fill.
- **Body Slate** (body): running text on light (11.5:1).
- **Soft Slate** (soft): ledes, helper text, the wordmark's place line (6.6:1).
- **Graphite Navy** (navy): the services and closing bands, the Facebook row.
- **Deep Navy** (deep): the how-it-works band, footer and hero base, always with the line texture except under the hero photo.
- **On-Dark** (on-dark) and **On-Dark Soft** (on-dark-soft): headings and body text on navy bands (9:1 and up).
- **Hairline** (line): the only divider, between the stacked "why" claims.

### Functional
- **Focus Blue** (focus): hover and focus outlines on form controls and light-ground buttons, caret colour. Deliberately not red, so a focused control never reads as an action fill.
- **Error** (error): inline error text and the error border on a bad field.

**The One Red Rule.** Red is the only hue on the page. Fills use Triquetra Red with white text; red as text picks the shade for its ground (Ink on light, Signal on dark or photo, Display only for large words on navy). Never put navy text on red.

**The Never Black Rule.** The logo's black is translated to graphite navy and deep navy. No surface is #000 or near it.

**The Accent Word Rule.** A heading may end in one accent-coloured phrase ("What we *transform.*", "How it *works.*", "you'll *love.*"), on dark bands and in the hero H1. Light-band headings stay all ink.

## Typography

**Display Font:** Cal Sans (with Avenir Next, Segoe UI, system-ui)
**Body Font:** the system sans stack (-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial)

**Character:** Cal Sans gives friendly, rounded geometric headings at a single weight; the system stack keeps reading text native and fast inside Facebook's in-app browser.

### Hierarchy
- **Display** (400, clamp 42–80px, 1.02): the hero H1 only, max 11ch on phones and 14ch on desktop, white on the photo.
- **Headline** (400, clamp 30–48px, 1.08): every section H2, `text-wrap: balance`.
- **Title** (400, clamp 20–22px, 1.15–1.2): one shared size for service rows, step titles, claims, the work-card caption and the Facebook row.
- **Button** (Cal Sans 400, 18px, 1): primary and ghost buttons, form labels and legends, the wordmark (22px phone, 25px desktop).
- **Lede** (system, clamp 17–19px): the line under a heading, max 38ch; the hero promise is 17–20px at 1.5, max 32ch/40ch.
- **Body** (system, 16px, 1.7): running text, inputs (16px so iOS never zooms), errors, the footer.
- **Label** (system, 14px, 1): the "(optional)" marks beside field labels.

**The One Size For Items Rule.** Anything that is an item in a list (row, step, claim, card caption) uses the Title size. No item invents its own size.

**The Single Weight Rule.** Cal Sans is only ever weight 400. Hierarchy comes from size and colour, not bolding.

## Layout

A single 1160px max-width container with a 20px gutter on phones and 40px from 760px up. Bands are full-bleed with 64px vertical padding on phones and 96px on desktop; the hero has its own 56/64px (phone) and 110/120px (desktop) padding.

Phones get one column throughout. At 760px the hero buttons sit side by side (240px minimum width) and services split into two columns. At 1024px sections become two-column splits with a 64px column gap: heading left and claims right; work heading and Facebook row left, 520px photo card right; the form's heading block sticks at 40px while the form scrolls; the three steps sit in a row with a 40px gap; the closing band puts the button bottom-right.

Heading blocks stack with a 16px gap and cap at 640px. Lists start 28–36px below their heading. Every tap target is 44px or more (rows 64px, buttons 56px, chips 48px, header icons 44px).

## Elevation & Depth

Flat by default. Depth comes from tonal bands (paper against navy against deep navy), the faint diagonal line texture on deep-navy bands, and translucent white tints on dark surfaces (6% service rows, 10–12% arrow circles). The hero gets depth from the real photo under a deep-navy gradient overlay (88% to 62% top to bottom), blurred 3px on phones so the railing never crosses the headline.

### Shadow Vocabulary
- **Float lift** (`box-shadow: 0 10px 28px rgba(10,14,22,.32)`): the floating Messenger circle only, because it sits over every band.

**The Flat Surfaces Rule.** Cards, rows, buttons and fields carry no shadow and no border at rest. Hover never adds a shadow.

**The Faint Lines Rule.** The deep-navy texture is `repeating-linear-gradient(135deg, transparent 0 22px, rgba(255,255,255,.035) 22px 23px)`: about 3.5% white, never stronger, so it never reads as lines through text. It belongs to deep-navy bands and the footer only.

## Shapes

Soft, rounded and borderless. Four radii, each with a job: full pills (999px) for every button, chip, arrow circle, step number and the floating circle; 24px for the quote form card and the work photo card; 18px for service rows and the Facebook row; 10px for text fields. The logo badge is shown as a circle. Borders only appear as 2px state strokes (focus blue, error) or the ghost button's 70% white outline.

## Components

### Buttons
- **Shape:** full pill, 56px tall, 26px side padding, Cal Sans 18px, optional 20px leading icon (Messenger glyph as inline SVG).
- **Primary:** Triquetra Red fill, white text, matching 2px border. Used for "Get a free quote", "Send on Messenger" (full width in the form) and "Message Kelluc Epoxy".
- **Hover / Focus:** hover darkens to Pressed Red (pointer devices only); press scales to 98%. On light grounds hover and focus add a 3px focus-blue outline at 3px offset; on dark grounds focus rings are Signal Red.
- **Ghost:** transparent with a 2px 70% white outline and on-dark text, for the second hero action; hover brightens the outline to white over a 10% white tint.
- **Quiet:** white fill, ink 2px outline, 48px, 16px text, for the copy-message fallback actions.

### Chips
- **Style:** Field Grey pills, 48px tall, ink text, no visible border at rest.
- **State:** hover gets a focus-blue 2px border; keyboard focus adds a 3px focus-blue outline at 2px offset; selected inverts to an ink fill with white text. Chips are the radio inputs for job and finish.

### Cards / Containers
- **Corner Style:** 24px.
- **Background:** white for the form card; the work card is a real photo with a bottom 45% gradient to 86% deep navy and a white Title caption on the photo.
- **Shadow Strategy:** none (see Elevation).
- **Border:** none.
- **Internal Padding:** clamp(20px, 5vw, 32px) on the form; the caption sits 22px in from the sides and 20px from the bottom.

### Inputs / Fields
- **Style:** Field Grey fill, 10px radius, 2px transparent border, 52px tall, 16px text, Cal Sans 18px label above with a 14px system "(optional)" mark.
- **Focus:** border turns focus blue; no glow.
- **Error:** border turns Error red and stays red while focused; the error is a plain sentence in Error red below the field.

### Navigation
- **Header:** paper, 68px (80px desktop); circular logo badge (48/52px) plus Cal Sans wordmark and an uppercase place line on the left, a 44px Facebook icon in ink on the right (hover Ink Red). A phone slot exists but stays hidden until a number is supplied. The header does not stick.
- **Footer:** deep navy with the line texture, name and area, and one Facebook link; links are 44px tall, hover to Signal Red.

### Service Rows
The services band's signature: each row is the link, on a 6% white tint with an 18px radius and a Title-size label, ending in a 44px arrow circle. **The Arrow Only Rule.** On hover only the arrow circle changes (fills Triquetra Red, white arrow); the row itself never changes background or gains a shadow. The same pattern serves the "see more of our work" Facebook row on paper, as a solid graphite navy block. One column on phones, two from 760px.

### Numbered Steps
Three steps on deep navy: a 48px Triquetra Red circle with a white Cal Sans numeral, a Title-size on-dark heading and an on-dark-soft line. Stacked on phones, three across from 1024px.

### Floating Messenger Circle
A 60px Triquetra Red circle, bottom right (16px plus safe-area insets), with a white 28px Messenger glyph and the Float lift shadow. It slides up (`.35s cubic-bezier(.2,.8,.2,1)`) once the hero has scrolled away and hides while the quote form is on screen, taking itself out of the tab order when hidden. One circle, never a bottom bar.

### Motion
- **Hero H1 bounce-in:** the hero H1 only. Letters slide in from 50px right, `1s cubic-bezier(.34,1.56,.64,1)`, 20ms apart; split in JS, words kept whole, accessible name preserved, original markup restored at the end.
- **Fade-up:** content below the first screen rises 12px and fades in over 400ms ease-out as it enters. Nothing is hidden without JS.
- **Reduced motion:** no bounce, no fade, no float slide, no smooth scroll; everything shows at rest.

## Do's and Don'ts

### Do:
- **Do** alternate full-bleed light and dark bands so each section starts with a change of ground; put the line texture on deep navy only.
- **Do** use Triquetra Red as a fill with white text, and pick Ink Red, Signal Red or Display Red by ground when red is text.
- **Do** keep focus and hover outlines on form controls in Focus Blue (3px, 3px offset), and Signal Red rings on dark grounds.
- **Do** use the Title size for every list item and Cal Sans at weight 400 only.
- **Do** keep tap targets at 44px or more and inputs at 16px or more.
- **Do** route every contact action to Facebook Messenger; the floating circle and the form never show at the same time.
- **Do** use real client photos under a deep-navy overlay, `object-fit: cover`, checking text contrast against the brightest pixel.

### Don't:
- **Don't** use black, or any near-black, as a surface.
- **Don't** introduce a second accent hue or a gradient fill on buttons.
- **Don't** put navy or ink text on a red fill.
- **Don't** use Display Red for small text.
- **Don't** add borders or shadows to cards, rows or buttons at rest, or a shadow on hover.
- **Don't** change a service row's background on hover; only its arrow circle responds.
- **Don't** animate any heading other than the hero H1, and don't hide content at opacity 0 without JS or under reduced motion.
- **Don't** raise the diagonal texture above about 4% white.

## House-style note

The page also ships four eyebrow pills (hero, why, work, quote): 14px, red dot, faint tint, no hover. They are Ellie's calm-style choice (pitch-site `calm-photo-style.md` item 5), kept on purpose even though Impeccable's craft floor bans eyebrows.
