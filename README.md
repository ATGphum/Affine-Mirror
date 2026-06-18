# Affine Mirror

A standalone design direction for **Affine** — the alignment layer for open intelligence.

Where Bittensor is the incentive layer that produces intelligence, Affine is the
mechanism that makes produced intelligence cumulative: it evaluates, aligns,
composes, validates, inherits, and reopens the frontier. This repo holds the
design doctrine and a set of self-contained page concepts that express that
posture.

## Contents

### Pages

Each page is a self-contained `.dc.html` design-canvas document. They share the
runtime in [`support.js`](support.js) and can be opened directly in a browser.

| File | Purpose |
| --- | --- |
| [`index.html`](index.html) | Landing page concept — the site root / default page |
| [`Affine Rationale.dc.html`](Affine%20Rationale.dc.html) | Longform rationale |
| [`Affine Dashboard.dc.html`](Affine%20Dashboard.dc.html) | Product / mechanism dashboard |
| [`Affine Design System.dc.html`](Affine%20Design%20System.dc.html) | Design system & tokens |
| [`Affine About.dc.html`](Affine%20About.dc.html) | About / overview |

### Docs

Strategy and visual rules, written to stand alone from any prior Affine project:

- [`uploads/AFFINE_ALIGNMENT_MIRROR_DOCTRINE.md`](uploads/AFFINE_ALIGNMENT_MIRROR_DOCTRINE.md)
  — strategy, message, posture, page intent, and review criteria.
- [`uploads/AFFINE_ALIGNMENT_MIRROR_VISUAL_SYSTEM.md`](uploads/AFFINE_ALIGNMENT_MIRROR_VISUAL_SYSTEM.md)
  — color, type, layout, components, page structure, and implementation rules.

### Assets

- `assets/` — the Affine brand mark (`affine-mark.png`, `affine-mark-clean.png`).
- `uploads/` — reference images and the doctrine docs.
- `.thumbnail` — preview image (PNG).

## Viewing

Open any `.dc.html` file in a browser, or serve the directory locally:

```sh
python3 -m http.server 8000
# then visit http://localhost:8000/  (serves the landing page)
```

## Runtime

[`support.js`](support.js) is **generated** from a separate `dc-runtime`
TypeScript source (`dc-runtime/src/*.ts`), which is not included here. Do not
edit `support.js` by hand; it is rebuilt with `bun run build` in that project.

## Design posture

> Black is the field, white is the theorem, gold is earned.

Restraint is the design. The direction mirrors Bittensor's seriousness, spacing,
and protocol-paper rhythm, and translates it into Affine's opposite pole. See the
doctrine for where this design mirrors Bittensor and where it deliberately
departs.
