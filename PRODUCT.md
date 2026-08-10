# PRODUCT.md

## What this is

A single-page, Romanian-language operating guide for the **Behringer X32 (full-size, 25 faders)** digital mixing console, used by the volunteer sound team of a church. It is published as a static `index.html` on GitHub Pages. No build step, no framework, no backend.

## Unique mechanism

It replaces "ask the person who knows" with a guide that maps the *whole* signal path — from the microphone on stage to the speakers in the hall — onto the specific buttons on this specific console, so a volunteer who has never touched a mixer can run a service without breaking anything.

## Audience and scene

**Primary reader:** a church sound volunteer, beginner to intermediate, not a trained audio engineer. Often young. Romanian speaker.

**The real scene (this drives every decision):** sitting at the mixing desk, **phone in one hand**, minutes before or *during* the service. Something is wrong, or they are about to do something they are unsure of, and other people are waiting. The room is **never dark** — it has plenty of daylight, and when it doesn't, plenty of artificial light. The phone screen is competing with a lit room, not lighting up a dark one.

Consequences:
- Mobile-first is literal, not a slogan. Desktop is the secondary case (learning at home, rehearsal).
- Light by default is a functional requirement, not a style preference: a dark screen in a bright room is the harder read, and it picks up every reflection. The OS `prefers-color-scheme` is deliberately **not** followed, because a phone set to system dark would otherwise hand the volunteer the worse screen.
- Night mode stays available as a secondary option, but nothing is designed around it.
- Reaching an answer must take seconds and one thumb, not reading.
- Every instruction must name the physical control by the label printed on the console.

**Secondary reader:** the same person at home or at rehearsal, reading to learn, unhurried.

## What success looks like

- A panicked volunteer finds "nu se aude nimic" and the first thing to check in under 10 seconds, one-handed.
- A new volunteer understands where sound *goes* before touching anything.
- Nobody sends a loud pop through the speakers or leaves `SENDS ON FADER` engaged.

## Content truth

- Source material: the operator's own earlier tutorial notes (signal chain + 8 numbered actions + a hand-drawn system sketch), plus the **official Behringer X32 User Manual** (75 pages, committed in this repo as `Behringer_X32_User_Manual.pdf`).
- Every procedural claim must be checkable against that manual. Where the manual is silent, the guide may state accepted live-sound practice, but must not invent console behaviour, menu paths or button names.
- The console is the **full-size X32**: 32 mic preamps, 16 mix buses, 6 matrix, 8 DCA groups, 6 mute groups, 25 faders (16 channel + 8 group + main).
- There is **no fixed channel assignment** at this church — channel numbers change from service to service, so the guide must never say "channel 1 is the preacher".

## Constraints

- Romanian, with correct diacritics (ă â î ș ț). Any typeface must render them properly.
- Single self-contained `index.html`, deployable to GitHub Pages as-is (`.nojekyll` present).
- Must work on an old Android phone over church Wi-Fi. No heavy assets, no framework.
- Accessible: real headings, real buttons, keyboard reachable, WCAG AA contrast.

## Explicitly not wanted

- The look of a generic AI-generated marketing site: gradient blobs, gradient headlines, pill badges, glassmorphism, decorative "tags" that carry no information.
- Gamification. Progress bars and "mark as learned" badges were tried and judged noise for a reference document.
- Anything that reads as unprofessional or padded. Content should be trimmed, not expanded.

## Voice

Direct, calm, imperative. Speaks to one person. Says what to press and what happens. Never hedges, never lectures. Safety warnings are stated once and plainly.
