---
version: 1
slug: "index-html"
primary_target: "index.html"
related_targets: []
---

# Portafolio — index.html

Scope: single-page personal portfolio. Visitor mode: Experience (the work leads).
Audience: recruiters (práctica / junior) and clients wanting automation, equally. Action: write by email (or phone). Proof: the four real projects; Kine screenshots and Softland diagram are the only real images. Constraints: single static HTML file, Spanish, copy rewritten shorter keeping every fact, Mac-inspired but copying nothing (no Apple logos, fonts, device mockups, traffic lights, "one more thing").

## Direction contract

THESIS: A keynote stage. The page is a dark stage and the work only becomes fully visible when the light finds it; refuses the category default of a light grid of project cards with a split hero.

OWN-WORLD: Pure black stage (#000 to #0a0a0a), white light as the only "color"; a soft white follow-spot cone (radial light with grain-free falloff) is the aura. Type: Host Grotesk, very large tight display, quiet small body in gray-white. Hairline rules at 10–14% white. One inverted act (white paper, black ink) for method, formal contrast. Mono (JetBrains Mono) only for real data: the agent's log, dates, figures.

STORY: Visitor learns in one viewport who Iván is and sees real software under the light; understands he already delivered to a real client and builds agents with a human in charge; writes to him.

FIRST VIEWPORT: Black stage; spotlight blooms from above center on load. Center: name line small, headline 2 lines at display scale, one-line lead, two actions (primary white pill "Escribirme", secondary text link "Ver proyectos"). Bottom 30% of the viewport: the Kine app screenshot rising into the light, dim until lit.

FORM: Escenario keynote — candidate 1 of my ordered list, chosen by the user as IMPECCABLE'S PICK over assigned candidate 3. seed:1e947704f186c3f2. Signature interaction: the follow-spot — screenshots and project scenes go from dim/desaturated to lit as they cross the stage center; pointer gently steers the hero spot on desktop; statement words light up with scroll. Raises: Nixie (real figures in fixed tabular digits), Viewfinder (center kept empty for the subject), Tanaka (monumental figure, whisper caption).

FINISH: unreviewed and undocumented is unfinished; this build ends with the finish review, the verdict, DESIGN.md, and every shipping raster carrying its provenance

## Decisions

- Softland: the live agent panel replaces img/diagrama-softland.svg on the page. The SVG uses a teal/violet palette that breaks the black-and-white world, and the panel draws the same flow (Softland, then the Python agent, then Excel and the printer, with the backend as next phase) with its demo data labeled. The SVG stays in img/ as source evidence.
- The cane and Roblox projects have no images, so they ship as typographic scenes with specs, not decorative stand-ins.
