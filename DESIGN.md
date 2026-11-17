---
name: Iván Jorquera
description: Portafolio personal. Un escenario negro donde el trabajo solo se ve del todo cuando lo encuentra la luz.
colors:
  stage: "#000000"
  light: "#ffffff"
  ink: "#fafafa"
  ink-dim: "rgba(250, 250, 250, 0.66)"
  ink-whisper: "rgba(250, 250, 250, 0.5)"
  rule: "rgba(250, 250, 250, 0.12)"
  rule-strong: "rgba(250, 250, 250, 0.2)"
  paper: "#f3f3f1"
  paper-ink: "#0a0a0a"
  paper-ink-dim: "#4d4d4b"
  paper-rule: "rgba(10, 10, 10, 0.14)"
typography:
  display:
    fontFamily: "Host Grotesk, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(42px, 7vw, 92px)"
    fontWeight: 600
    lineHeight: 0.98
    letterSpacing: "-0.04em"
  headline:
    fontFamily: "Host Grotesk, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(40px, 6.4vw, 84px)"
    fontWeight: 600
    lineHeight: 1
    letterSpacing: "-0.04em"
  statement:
    fontFamily: "Host Grotesk, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(34px, 5.6vw, 72px)"
    fontWeight: 500
    lineHeight: 1.06
    letterSpacing: "-0.035em"
  title:
    fontFamily: "Host Grotesk, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(34px, 4.8vw, 62px)"
    fontWeight: 600
    lineHeight: 1.02
    letterSpacing: "-0.035em"
  quote:
    fontFamily: "Host Grotesk, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(28px, 3.8vw, 50px)"
    fontWeight: 300
    lineHeight: 1.12
    letterSpacing: "-0.03em"
  lead:
    fontFamily: "Host Grotesk, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(17px, 1.6vw, 20px)"
    fontWeight: 400
    lineHeight: 1.55
  body:
    fontFamily: "Host Grotesk, Segoe UI, system-ui, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "Host Grotesk, Segoe UI, system-ui, sans-serif"
    fontSize: "13px"
    fontWeight: 400
    lineHeight: 1.45
    letterSpacing: "0.01em"
  data:
    fontFamily: "JetBrains Mono, ui-monospace, Consolas, monospace"
    fontSize: "13px"
    fontWeight: 400
    lineHeight: 1.75
    fontFeature: "\"tnum\""
rounded:
  pill: "999px"
  panel: "16px"
  node: "12px"
  focus: "6px"
spacing:
  gutter: "clamp(16px, 4vw, 48px)"
  max: "1200px"
  bar: "56px"
  act: "clamp(96px, 16vh, 180px)"
  scene: "clamp(96px, 14vh, 160px)"
  column-gap: "clamp(32px, 6vw, 96px)"
components:
  button-primary:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.stage}"
    typography: "{typography.body}"
    rounded: "{rounded.pill}"
    padding: "16px 28px"
  button-primary-hover:
    backgroundColor: "{colors.light}"
    textColor: "{colors.stage}"
  nav-pill:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.stage}"
    rounded: "{rounded.pill}"
    padding: "7px 14px"
  link-text:
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    padding: "10px 2px"
  chip-copy:
    textColor: "{colors.ink-dim}"
    rounded: "{rounded.pill}"
    padding: "6px 14px"
  chip-copy-hover:
    textColor: "{colors.ink}"
  nav-bar:
    backgroundColor: "{colors.stage}"
    textColor: "{colors.ink-dim}"
    height: "56px"
  agent-panel:
    textColor: "{colors.ink-dim}"
    rounded: "{rounded.panel}"
  flow-node:
    textColor: "{colors.ink}"
    rounded: "{rounded.node}"
    padding: "14px 16px"
  flow-node-core:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.stage}"
    rounded: "{rounded.node}"
    padding: "14px 16px"
  paper-act:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.paper-ink}"
---

# Design System: Iván Jorquera

## Overview

**Creative North Star: "The Keynote Stage"**

The page is a dark stage, and the work only becomes fully visible when the light finds it. White light is the only color. A soft follow-spot (a blurred cone, a pool where it lands, and a hot source above the frame) is the system's aura. Everything else is black, white, and the grays that light makes as it falls off. Real software (the Kine screenshots, the Softland agent panel) sits under the light. Projects without imagery stand on the stage as type and specs, with no decorative stand-ins.

The system is quiet and formal. Display type is very large, tight and set in two voices: a lit clause and a dim clause. Body text is small, gray-white and set to measure. Hairline rules at 12% white do the structural work that boxes and cards would do elsewhere. One act per page flips to white paper with black ink for formal contrast, and the stage darkens back over it as you leave.

The build follows the direction contract with one difference: the first viewport's name is not its own small line above the headline. It is set inside the lead in full ink ("Soy **Iván Jorquera**…"). The build is the authority here.

**Key Characteristics:**
- Pure black stage, white light as the only color, no hue anywhere.
- Follow-spot light: media and scenes go from dim and desaturated to lit as they cross the center of the viewport.
- Two-voice display headlines: a lit clause, then a dim clause.
- Hairline rules instead of cards; projects are scenes, not tiles.
- Exactly one inverted paper act.
- Mono is reserved for real data: logs, timestamps, dates, phone numbers, file names.

## Colors

The palette is a monochrome of light on black. Each value is the stage, or the light, or the light at some strength.

### Primary
- **Stage Light** (`light`): the follow-spot color, used through the `--light` channel at low alpha for cones, pools, scene halos and glows. Pure white also marks hover on filled buttons.
- **Lit Ink** (`ink`): headlines, emphasized words in body copy, filled pill buttons, the agent's core node, focus rings and selection.

### Neutral
- **Stage Black** (`stage`): the page, the fixed bar and the text on filled buttons.
- **Dim Ink** (`ink-dim`, 66% white): body paragraphs, leads, nav links at rest, agent chrome.
- **Whisper Ink** (`ink-whisper`, 50% white): the dim clause of headlines, captions, spec labels, timestamps, footer and log history.
- **Hairline** (`rule`, 12% white): section, spec, sheet and footer dividers, and the bar's bottom edge.
- **Strong Hairline** (`rule-strong`, 20% white): borders on objects that sit on the stage, such as screenshot glass, flow nodes, wires and the copy chip.
- **Paper** (`paper`): the background of the one inverted act.
- **Paper Ink** (`paper-ink`) / **Paper Dim** (`paper-ink-dim`) / **Paper Rule** (`paper-rule`): ink, dim clause and secondary text, and hairlines on paper.

### Named Rules
**The Single Light Rule.** No hue, anywhere. Any asset that carries color is replaced or left out. The teal and violet Softland diagram was replaced by a live monochrome panel for this reason.

**The Two-Voice Rule.** Display and section headlines put their second clause in Whisper Ink on stage, or Paper Dim on paper. The lit clause states and the dim clause qualifies.

## Typography

**Display Font:** Host Grotesk (with Segoe UI, system-ui)
**Body Font:** Host Grotesk
**Label/Mono Font:** JetBrains Mono, for data only

**Character:** One grotesk in every role. Display sizes are tight and heavy, with negative tracking down to -0.04em. Body text is light, gray and generous. The mono is the instrument voice, and it only ever reports.

### Hierarchy
- **Display** (600, clamp 42–92px, 0.98): the hero headline and the finale headline (which runs to 96px). Balanced wrap, max 14–22ch.
- **Headline** (600, clamp 40–84px, 1): the opening heading of each act. Max 16ch, two voices.
- **Statement** (500, clamp 34–72px, 1.06): the pinned scroll statement. Its words light up one at a time as you scroll, from 16% to full opacity.
- **Title** (600, clamp 34–62px, 1.02): project scene names. Method tenets use a smaller step (clamp 28–48px).
- **Quote** (300, clamp 28–50px, 1.12): the one blockquote on paper. The light weight is the formal register.
- **Lead / Body** (400, 17–20px and 17px, 1.55; body drops to 16px below 560px): Dim Ink, max 44–70ch, pretty wrap.
- **Label** (400, 13px): spec labels, captions ("whisper") and footer, in Whisper Ink, sentence case.
- **Data** (JetBrains Mono 13–14px): the agent log, timestamps, years, phone number and email line.

### Named Rules
**The Mono-Is-Data Rule.** Mono appears only where the content is machine or record data. It is never a decorative label voice.

**The Tabular Figures Rule.** Real figures (years, counts, intervals, phone numbers) are set in tabular numerals so they hold position like an instrument readout.

## Layout

The layout is a single centered column with a max width of 1200px and a fluid gutter of 16–48px. The page is a sequence of acts: hero, pinned statement (200vh tall with a 100vh sticky frame), projects, the paper act, the technical sheet, and the finale. Acts breathe with 96–180px of vertical padding. Project scenes step down with 96–160px between them.

Inside an act, text pairs sit on a two-column grid (1.15fr / 1fr or 1fr / 1fr) with a 32–96px gap, aligned to the end or the baseline. The technical sheet uses a 0.7fr / 2fr label/content grid, with a three-track row for name, detail and year. Specs are a three-column definition list under a hairline. The fixed bar is 56px, and anchors offset by the same 56px.

The hero and finale are center-aligned with the spotlight behind. Every other act is left-aligned. Below 860px all grids collapse to one column, specs stack with hairlines between them, and the agent flow turns vertical. Below 640px the nav keeps only the "Escribirme" pill.

## Elevation & Depth

Depth is light, not shadow. A surface reads as raised because light falls on it: a white glow spills beneath lit objects and grows with their `--lit` value. Dark shadow is used only to seat the screenshot glass on the stage. The page itself is flat black, and the follow-spot (blurred cone, pool, source) is the only atmospheric layer.

### Shadow Vocabulary
- **Button glow** (`0 10px 40px -12px rgba(255,255,255,0.45)`, hover `0 16px 50px -12px rgba(255,255,255,0.6)`): white light pooling under the primary pill.
- **Screen light** (`0 50px 120px -30px rgba(255,255,255, lit × 0.22), 0 30px 60px -20px rgba(0,0,0,0.9)`): screenshot glass, lit from above and seated on black.
- **Panel light** (`0 50px 120px -40px rgba(255,255,255, lit × 0.18)`): the agent panel.
- **Node flare** (`0 0 30px -6px rgba(255,255,255,0.5)`): a flow node while it is active.

### Named Rules
**The Light-Not-Shadow Rule.** Elevation is a white glow from the light above, scaled by how lit the object is. Never use hard or offset shadows.

**The Follow-Spot Rule.** Stage objects carry a `--lit` value from 0 to 1, driven by their distance from the center of the viewport. At low light they dim (brightness down to 30%), desaturate, tilt back up to 14° and shrink slightly. When lit they are full color, flat and glowing. With reduced motion, everything stays fully lit and untransformed.

## Shapes

Two shapes do almost all the work: full pills for anything you press, and soft rectangles for objects on the stage. Screenshot glass uses 10–16px corners, the agent panel 16px, and flow nodes 12px. Borders are 1px hairlines in white at 12–20% strength. A dashed hairline marks something not yet built (the agent's "next phase"). Structure comes from horizontal rules running the full width of the column, never from enclosing boxes. Icons are 18px line SVGs with a 1.6 stroke and round caps.

## Components

### Buttons
- **Shape:** full pill (999px).
- **Primary:** Lit Ink fill, Stage Black text, 500 weight at 17px, 16px × 28px padding, with a white glow beneath.
- **Hover / Focus:** turns pure white, lifts 1px and the glow strengthens. Press scales to 0.98 in 80ms. Focus is a 2px ink outline offset 4px.
- **Text link (secondary):** Lit Ink, no underline at rest. On hover the label underlines and the arrow drops 3px.

### Chips
- **Copy chip:** an outline pill with a Strong Hairline border, 14px label and line icon. On hover or confirmation the border and text go to full ink, and the copy icon swaps to a check.

### Cards / Containers
- **Screen glass:** a screenshot in a 10–16px rounded frame with a Strong Hairline border and no window chrome. It is lit by the follow-spot. Caption below in Label.
- **Agent panel:** 16px corners, near-black vertical gradient (#0d0d0d to #050505), Strong Hairline border. The mono header has a status dot that glows when running. A 2px progress tick runs the 10-second cycle. Below that are the flow diagram and a mono log that fades in from the top, then a footer note.
- **Spec list:** three label/value pairs under a hairline, label in Whisper Ink 13px and value at 15px.

### Navigation
- **Bar:** fixed, solid Stage Black, 56px tall, hairline bottom edge. Brand at 600 weight 16px on the left. Links at 14px in Dim Ink, going to ink on hover and for the active section. The CTA is a small ink pill (7px × 14px).
- **Mobile:** below 640px only the brand and the pill remain.

### Flow Diagram (signature)
The flow is a row of nodes joined by hairline wires: source, then a core node (inverted to an ink fill), then the outputs. A node flares while active, and a glowing pulse travels along each wire as data moves. Below 860px the diagram turns vertical. The flow is labeled as a simulation with example data.

### Paper Act (signature)
The one inverted section: Paper background with Paper Ink. Tenets sit in a two-column row between paper hairlines, and the act closes on a light-weight blockquote. A stage-black overlay fades out as the act reaches the viewport, so the room "lights up" on entry and darkens again on exit.

## Do's and Don'ts

### Do:
- **Do** keep the stage pure black (#000000) and let the follow-spot be the only atmosphere.
- **Do** split display and section headlines into a lit clause and a dim clause.
- **Do** put real software under the light: screenshots and live, honest panels, each labeled when its data is example data.
- **Do** separate content with full-width hairlines at 12% white, and border stage objects at 20%.
- **Do** use mono only for data, and tabular numerals for every real figure.
- **Do** keep every lit element fully lit and static when reduced motion is requested.

### Don't:
- **Don't** introduce any hue: no accent color, no colored diagrams, no tinted grays.
- **Don't** box projects in cards or a tile grid. A project is a scene under its own light, with a hairline spec list.
- **Don't** use hard or offset shadows. Depth is white light from above.
- **Don't** use more than one inverted paper act per page.
- **Don't** copy Apple: no Apple logos, Apple system fonts, device mockups, window traffic lights or borrowed keynote catchphrases.
- **Don't** invent stand-in imagery for projects that have none. Set them as typographic scenes.
