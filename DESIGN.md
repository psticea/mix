---
name: Ghid X32
description: A wayfinding sign system for a church sound team operating a Behringer X32.
colors:
  sign-yellow: "#FFCC00"
  sign-black: "#0B0B0B"
  prohibition-red: "#D93A25"
  safe-green: "#17A05B"
  night-sign-yellow: "#E3B300"
  night-ground: "#1A1917"
  night-panel: "#232220"
  night-panel-raised: "#2A2925"
  night-rule: "#3D3C36"
  night-ink: "#E9E7DE"
  night-ink-muted: "#9E9D95"
  night-ink-faint: "#96948B"
  day-ground: "#E6E6E6"
  day-panel: "#FFFFFF"
  day-panel-raised: "#F4F4F2"
  day-rule: "#C6C6C1"
  day-ink: "#0B0B0B"
  day-ink-muted: "#55544F"
  day-ink-faint: "#63625C"
typography:
  display:
    fontFamily: "Fira Sans, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, sans-serif"
    fontSize: "clamp(2.6rem, 1.6rem + 5vw, 4.6rem)"
    fontWeight: 800
    lineHeight: 0.9
    letterSpacing: "-0.045em"
    fontFeature: "tabular-nums"
  headline:
    fontFamily: "Fira Sans, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, sans-serif"
    fontSize: "clamp(1.35rem, 1.05rem + 1.5vw, 2.05rem)"
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: "-0.015em"
  title:
    fontFamily: "Fira Sans, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, sans-serif"
    fontSize: "1.08rem"
    fontWeight: 700
    lineHeight: 1.3
    letterSpacing: "-0.01em"
  body:
    fontFamily: "Fira Sans, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, sans-serif"
    fontSize: "clamp(1.02rem, 0.97rem + 0.28vw, 1.12rem)"
    fontWeight: 400
    lineHeight: 1.62
    letterSpacing: "normal"
  dense:
    fontFamily: "Fira Sans, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, sans-serif"
    fontSize: "0.99rem"
    fontWeight: 400
    lineHeight: 1.55
    letterSpacing: "normal"
  secondary:
    fontFamily: "Fira Sans, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, sans-serif"
    fontSize: "0.93rem"
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: "normal"
  caption:
    fontFamily: "Fira Sans, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, sans-serif"
    fontSize: "0.86rem"
    fontWeight: 400
    lineHeight: 1.45
    letterSpacing: "normal"
  control:
    fontFamily: "Fira Sans, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, sans-serif"
    fontSize: "0.76rem"
    fontWeight: 700
    lineHeight: 1
    letterSpacing: "0.1em"
  micro:
    fontFamily: "Fira Sans, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, sans-serif"
    fontSize: "0.68rem"
    fontWeight: 700
    lineHeight: 1
    letterSpacing: "0.14em"
  numeral:
    fontFamily: "Fira Sans, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, sans-serif"
    fontSize: "1.45rem"
    fontWeight: 800
    lineHeight: 1
    letterSpacing: "-0.03em"
    fontFeature: "tabular-nums"
  label:
    fontFamily: "Fira Sans, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, sans-serif"
    fontSize: "clamp(0.68rem, 0.65rem + 0.12vw, 0.75rem)"
    fontWeight: 700
    lineHeight: 1
    letterSpacing: "0.14em"
  diagram:
    fontFamily: "Fira Sans, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, sans-serif"
    fontSize: "15px"
    fontWeight: 700
    lineHeight: 1
    letterSpacing: "0.02em"
rounded:
  none: "0"
spacing:
  hair: "4px"
  xs: "8px"
  sm: "13px"
  md: "16px"
  lg: "22px"
  xl: "30px"
components:
  destination-row:
    backgroundColor: "{colors.sign-yellow}"
    textColor: "{colors.sign-black}"
    typography: "{typography.headline}"
    rounded: "{rounded.none}"
    padding: "14px 16px"
  destination-row-alarm:
    backgroundColor: "{colors.prohibition-red}"
    textColor: "#FFFFFF"
    rounded: "{rounded.none}"
    padding: "14px 16px"
  area-band:
    backgroundColor: "{colors.sign-yellow}"
    textColor: "{colors.sign-black}"
    typography: "{typography.headline}"
    rounded: "{rounded.none}"
    padding: "12px 16px"
    nightVariant: "transparent face, 2px {colors.sign-yellow} bottom rule, numeral in {colors.night-sign-yellow}"
  gantry-index:
    backgroundColor: "{colors.sign-yellow}"
    textColor: "{colors.sign-black}"
    typography: "{typography.label}"
    rounded: "{rounded.none}"
    padding: "0 16px"
    height: "60px"
  gantry-emergency:
    backgroundColor: "{colors.prohibition-red}"
    textColor: "#FFFFFF"
    typography: "{typography.label}"
    rounded: "{rounded.none}"
    padding: "0 14px"
    height: "60px"
  notice-stop:
    backgroundColor: "{colors.prohibition-red}"
    textColor: "#FFFFFF"
    rounded: "{rounded.none}"
    padding: "13px 15px"
  pictogram:
    backgroundColor: "{colors.sign-black}"
    textColor: "#FFFFFF"
    rounded: "{rounded.none}"
    size: "38px"
  keycap:
    backgroundColor: "{colors.night-panel-raised}"
    textColor: "{colors.night-ink}"
    rounded: "{rounded.none}"
    padding: "0.08em 0.42em"
---

# Ghid X32 — Design System

## Overview

**North star: an international airport sign system, in a lit terminal.**

This is not a documentation site. The reader is a volunteer sitting at a mixing
desk, on a phone, minutes before a service starts. They are not reading — they
are navigating a building under time pressure. So the surface behaves like
terminal signage: a junction board of numbered destinations, a gantry sign that
always tells you where you are, monumental numerals visible from a distance,
pictograms instead of decoration, and one route drawn as a transit line.

Three rules follow from that and govern everything else:

1. **Yellow is wayfinding, and nothing else.** It marks where to go and where you
   are. The moment yellow decorates a paragraph, the sign system stops working.
   It is also *rationed by mode*: in daylight a full yellow sign face is exactly
   right and the section bands wear it. At night seven full slabs became seven
   glowing walls, so there the band keeps only its numeral and a lit rule.
2. **Everything is a panel, not a card.** Hard rectangles, hairline frames, zero
   decorative radius, no shadows, no gradients. Depth comes from ground/panel
   value separation, never from blur.
3. **Day is the default.** The room is never dark — it has daylight, or it has
   the lights on. A dark screen there is the harder read and catches every
   reflection, so light leads and the system preference is not followed. Night
   mode exists for the person reading at home in the evening.

The visual world is deliberately the opposite of the site it replaced (gradient
blobs, gradient headlines, pill tabs, badge rows, rounded cards, blue/purple
accent) — the generic AI-default look the client rejected by name.

## Colors

| Role | Token | Value | Use |
|---|---|---|---|
| Wayfinding | `sign-yellow` | `#FFCC00` day / `#E3B300` night | Sign panels, the board, section numerals and rules, the active route station, the index button. **Never body copy, never a border for emphasis, never a hover tint.** |
| Sign ground | `sign-black` | `#0B0B0B` | Pictogram inset squares, type on yellow, step numerals. |
| Prohibition | `prohibition-red` | `#D93A25` (both modes) | Only for "this will hurt the service": the emergency route (07), STOP notices, the emergency shortcut in the gantry. |
| Safe | `safe-green` | `#17A05B` | Completed checklist items and GO notices. Nothing else. |
| Ground / panel / ink | `night-*`, `day-*` | see frontmatter | Every neutral resolves through `--ground`, `--panel`, `--panel-raised`, `--rule`, `--ink`, `--ink-muted`, `--ink-faint`. |

Both modes are declared as token blocks on `html[data-mode="night"|"day"]`.
Component CSS references the semantic token only, so a mode never needs a
component override — with two deliberate exceptions. `.area-band` changes
treatment between modes (lit face by day, lit edge at night), because a sign
genuinely does look different depending on how much light is on it. And yellow
numerals set on the page ground (`.next-n`, `.gantry-now .g-num`) switch to
`--ink` in day mode: yellow type cannot carry contrast on a light surface, so
on light the colour lives in the rule and the numeral goes black.

Night is not "day with the lights off". It is the same sign system dimmed: the
ground lifts off pure black to a warm charcoal, and the yellow drops in
*lightness only* — `#FFCC00` is `hsl(48,100%,50%)`, the night face is
`hsl(47,100%,45%)`. Hue and chroma are untouched on purpose. Desaturating a
signage yellow to calm it down produces mustard, which reads as dirty rather
than dimmed. Red is identical in both modes: it was never the glare source, and
one red keeps "stop" unambiguous.

Contrast floor is WCAG AA in both modes, verified by measurement rather than by
eye. Three token values are set by that floor, not by taste:

- `prohibition-red` is `#D93A25` because white body text on it must clear 4.5:1
  (it lands at 4.58). A lighter red looked better and failed.
- `night-ink-faint` `#96948B` and `day-ink-faint` `#63625C` are the lightest and
  darkest values that keep 11px uppercase micro-copy legible on `--ground`.
  `--ink-faint` is a *text* tier, so it may never be dimmed further.

Yellow-on-black and black-on-yellow both clear AAA.

`@media print` re-declares the neutral tokens on
`html, html[data-mode="night"], html[data-mode="day"]`, not on `:root` — the
mode selectors outrank `:root`, so a `:root` print override silently loses and
night ink ends up on white paper.

## Typography

**Fira Sans, one family, three weights (400/700/800).** A humanist grotesque
in the Frutiger lineage — the tradition airport signage actually comes from —
with complete Romanian diacritic coverage (ă â î ș ț). Self-hosted as woff2
(latin + latin-ext), so the page makes zero third-party requests. There is no
second family and no monospace: console button names are set in the same face
inside an engraved keycap, so the page never has to spend yellow or a second
font on them.

Hierarchy is carried by **weight and scale**, never by color. The ramp is
closed — every size in the stylesheet is one of these tokens, there are no
one-off literals:

- `display` (800) — destination numerals only. Tabular, tightly tracked, set to
  be read at arm's length in a dark room. `--t-num`, with `--t-num-sm` for the
  overlay and `--t-band` for area bands.
- `headline` (700) — destination names and area titles.
- `numeral` (800, `--t-xl`) — row numbers and the "Urmează" figure.
- `title` (700, `--t-lg`) — expandable row titles, section subheads, next-sign
  names.
- `body` (400, 1.62 line-height, 66ch measure) — running prose. `--t-body`.
- `dense` (400, `--t-md`) — numbered steps and row bodies, where a paragraph is
  a procedure rather than prose.
- `secondary` (400, `--t-sm`) — legend copy, checklist counter, footer.
- `caption` (400, `--t-xs`) — destination subtitles and row subtitles.
- `control` (700, 0.1em tracking, uppercase, `--t-mini`) — buttons and mode
  switches.
- `micro` / `label` (700, 0.14em tracking, uppercase, `--t-micro` /
  `--t-label`) — signage micro-copy: "DESTINAȚIA", "INTRARE", zone names.
  Uppercase is reserved for these two roles.
- `diagram` (700) — lettering inside the SVG schematics, in user units so it
  scales with the drawing: `--t-dia-n` 18, `--t-dia-t` 15, `--t-dia-i` 13,
  `--t-dia-s` 11.5, `--t-dia-k` 11.

## Layout

- Container `1160px`, gutters `16px`, reading measure `66ch` inside rows.
- Single column at every width. Two columns appear in exactly one place: the
  landing board at ≥900px, where destinations pair up and the emergency row spans
  both.
- **Breakpoints: 760px** (diagrams switch from the narrow drawing to the wide
  drawing; footer splits) and **900px** (the gantry moves from the bottom of the
  screen to the top).
- The gantry is fixed at **60px** and reserves its own space via body padding, so
  nothing is ever hidden under it. On phones it sits at the bottom — inside the
  thumb zone, because the reader is holding the phone one-handed at a desk. On
  desktop it becomes an overhead sign at the top, where terminal signage belongs.
- Vertical rhythm uses `clamp()` between sections so the phone view stays dense
  and the desktop view breathes.

## Elevation & Depth

**There are no shadows in this system.** Not one `box-shadow`, no blur, no glow.
Depth is signage depth:

- `ground` → `panel` → `panel-raised` value steps.
- **1px hairline rules** as the only separator.
- Pictograms in solid black inset squares — the sign is *cut into* the panel.
- The only "lit" surface is the yellow itself, and it is lit by being pure, not by
  being glowed.

Motion is equally restricted: one **split-flap** animation on the gantry's
destination readout (0.26s, staggered per character), which is how a real
departures board updates, plus a 0.18s chevron rotation. Everything collapses
under `prefers-reduced-motion`.

## Shapes

- **`border-radius: 0` everywhere.** No exceptions, including buttons, inputs,
  checkboxes and the keycaps.
- Arrows are locked to the edge they point past, never centered as ornament.
- Pictograms are 38px black squares (30px inside notices); the glyph is white,
  drawn on a 24px grid, single-color, no strokes.
- Diagrams are hand-authored inline SVG using the same token variables, so they
  re-color with the mode. They must read as *drawn schematics* — a line with
  stations, a room with nodes, a console seen from above — not as boxes with
  labels.

## Components

- **Board / destination row** — the landing page *is* the board. Monumental
  numeral, name, one-line subtitle, edge arrow. The emergency destination is red
  and always last.
- **Gantry** — fixed sign carrying: current destination (split-flap readout, also
  the button that opens the index), the yellow index button, the red emergency
  shortcut.
- **Board overlay** — the full destination list as a full-screen yellow board.
  Traps focus, closes on Escape, restores focus to the opener.
- **Area band** — every section opens with its number in yellow over a single
  lit rule, so a mid-page arrival still knows where it is without another
  full-bleed slab. Red numeral and rule for 07.
- **Entry row** — native `<details name="...">` so only one is open at a time,
  with a JS fallback. Content is real HTML, so browser find-in-page works.
- **Notice** — framed panel with a pictogram inset square. Three intents only:
  neutral (info), `stop` (solid red, prohibition), `go` (green pictogram, safe).
  Never more than one notice per row.
- **Route map** — the channel signal path drawn as a transit line with tappable
  stations; picking a station highlights the matching legend entry, and vice
  versa. Two hand-drawn SVGs (wide/narrow) rather than one that scales badly.
- **Checklist** — persists to `localStorage` (`x32.check.v2`) with a visible
  count and a reset. Green when done.
- **Keycap** — console buttons (`kbd`) as engraved chips. This is what keeps the
  yellow budget intact.

## Do's and Don'ts

**Do**

- Reserve yellow for wayfinding, red for danger, green for safe. Three signals,
  no more.
- Lead every instruction with a numbered step; the reader is executing, not
  studying.
- Draw new diagrams as inline SVG with the existing token classes so they follow
  the mode.
- Keep new content as static HTML — the reader may be searching the page, and the
  page must work with JS off.
- Check every change on a 390px viewport in day mode first. That is the real
  device.

**Don't**

- Don't add a hero, a headline block, badge pills, or tag chips. The client
  rejected them by name; the board is the entry point.
- Don't introduce a second font family, a monospace, or italics.
- Don't add rounded corners, shadows, gradients, or blur.
- Don't use color as the only carrier of meaning — every colored state also has a
  pictogram, a label, or a position.
- Don't publish a fixed channel map. Channel assignment changes per service; the
  guide teaches the method, and the concrete numbers are learned at the desk.
- Don't state as manual fact anything that is not in the official X32 manual;
  general practice is written as general practice.
