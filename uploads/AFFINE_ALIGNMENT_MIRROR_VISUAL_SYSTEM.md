# Affine Alignment Mirror Visual System

Canon 2.0 · Updated 2026-07-17

## Status

This document defines how the Affine Alignment Mirror direction is rendered and implemented.

Read with:

- `AFFINE_ALIGNMENT_MIRROR_DOCTRINE.md` for meaning and message
- `BITTENSOR_REFERENCE_2026-06-18.md` for the pinned external reference

The Doctrine controls meaning. This file controls execution. Existing HTML pages are examples and must be corrected when they diverge from these rules.

## Design Summary

Affine is the blackpaper counterpart to Bittensor's protocol-paper restraint:

| Reference behavior | Affine translation | Meaning |
| --- | --- | --- |
| white paper | `paper-black` field | blackpaper surface |
| black signal | white theorem and structure | proof |
| tau micro mark | Lambda signature | protocol shorthand |
| central network object | Affine monument or mechanism | unresolved field or judgment |
| incentive language | alignment and inheritance | cumulative progress |
| monochrome rigor | monochrome plus controlled exceptions | semantic discipline |
| longform whitepaper | longform blackpaper | protocol thesis |
| equations and figures | equations, thresholds, lineage | mechanism proof |
| silence | silence | authority through restraint |

The governing sentence is:

> Black paper. White theorem. Gold validation.

The full-spectrum monument is a contained exception (the Doctrine defines its meaning) and must not become a general page palette.

## Reference Version

Use the captures and measurements in `BITTENSOR_REFERENCE_2026-06-18.md`.

Do not require a designer to inspect the current live Bittensor site. The live site may change. If a newer state becomes strategically useful:

1. capture it
2. date it
3. document the changed observations
4. update the reference version in this file and the Doctrine

Never inherit a changing external design silently.

## Identity System

Affine uses three levels of identity.

### Monument

Asset:

```text
affine-mark-clean.png
```

Role:

- landing hero
- manifesto or rationale opener
- launch and poster composition
- rare full-page identity moment

Rules:

- preferred size: 180–460px depending on viewport and treatment
- minimum size: 96px
- preserve transparency and full-spectrum rendering
- allow slow spatial or resolving motion only when a still frame remains complete
- provide a static reduced-motion state
- keep the surrounding field monochrome

Do not sample the spectrum into gradients, charts, glows, borders, or secondary components.

### Everyday Mark

Asset:

```text
affine-mark-gold.png
```

Role:

- desktop and mobile navigation
- product UI and dashboards
- compact brand ownership
- chart or document authorship

Rules:

- minimum size: 24px
- preferred navigation size: 28–32px
- use `identity-gold`
- do not animate continuously
- do not treat its presence as a validated-state indicator

This is identity gold: it means “Affine,” not “approved.”

### Lambda Signature

Prototype form:

```text
Λ
```

Role:

- favicon
- footer
- document stamp
- tiny loading state
- compact protocol shorthand

Rules:

- minimum size: 16px
- preferred size: 16–24px
- use a tuned asset for production
- thicken the stroke below 24px
- use `identity-gold` or `ink-white`
- do not place it in a circle by default
- do not repeat it as a pattern

The hierarchy is:

```text
monument: full-spectrum mark
everyday identity: flat gold mark
smallest signature: Lambda
```

## Color System

### Core Tokens

```text
paper-black       #1C1C1C
void-black        #000000
ink-white         #F5F2EA
paper-white       #FFFFFF
soft-white        #D8D4C8
muted-white       #9B968B
quiet-white       #88847B
faint-white       rgba(245,242,234,0.18)
hairline-white    rgba(245,242,234,0.10)

affine-gold       #D6B85A
identity-gold     affine-gold
validation-gold   affine-gold
gold-muted        #A48B3B
gold-faint        rgba(214,184,90,0.20)

error-red         #C0705A
success-green     #6F9F7A
info-blue         #7C9AB8
```

The two gold channel tokens share `affine-gold`'s value while remaining semantically distinct in code.

Do not introduce undocumented text colors. In particular, do not use `#5E5A52` or darker gray for text on `paper-black`.

### Contrast Roles on `paper-black`

| Token | Approx. contrast | Permitted text role |
| --- | ---: | --- |
| `ink-white` | 15.2:1 | primary text, titles, equations |
| `soft-white` | 11.5:1 | secondary text, navigation |
| `muted-white` | 5.8:1 | captions, metadata, body-support text |
| `quiet-white` | 4.6:1 | lowest-priority normal text |
| `affine-gold` | 8.8:1 | earned state (`validation-gold`) and identity mark (`identity-gold`) |
| `gold-muted` | 5.1:1 | secondary gold labels |
| `error-red` | 4.6:1 | failure text with an icon or label |
| `success-green` | 5.6:1 | positive delta with an icon or label |
| `info-blue` | 5.8:1 | informational text |

Opacity tokens are for lines, fills, and non-text decoration unless the resulting contrast has been tested.

### Gold Channels

Gold is permitted in two channels. Both resolve to `affine-gold`.

**Identity gold (`identity-gold`)**

- everyday Affine mark
- Lambda signature

**Validation gold (`validation-gold`)**

- validated result
- selected candidate
- replacement event
- inherited baseline
- active frontier

Do not use gold for:

- current navigation
- hover or focus
- generic buttons
- generic selected controls
- section dividers
- decorative borders
- background glow
- premium or luxury mood

Current navigation uses `ink-white` plus an underline or equivalent non-color marker.

## Typography

The system is small, sparse, and paper-like.

Preferred stack, subject to licensing:

```text
Body / headings:
Haffer, HafferSQ, Helvetica Neue, Arial, sans-serif

Mono labels:
Fira Code, DM Mono, TTCommonsPro, SFMono-Regular, Menlo, Consolas, monospace

Equations:
KaTeX_Main, STIX Two Text, Times New Roman, serif
```

Safe fallback:

```text
Body / headings:
Inter, Helvetica Neue, Arial, sans-serif

Mono labels:
IBM Plex Mono, SFMono-Regular, Menlo, Consolas, monospace

Equations:
STIX Two Text, Times New Roman, serif
```

Do not assume fonts observed in the Bittensor reference are licensed for Affine.

### Type Roles

```text
navigation
  11px desktop / 10px compact
  mono 600
  0.08em tracking
  uppercase

hero theorem
  15–20px desktop / 14–17px mobile
  sans or mono
  500
  1.5 line-height
  560px max

page title
  30–42px desktop / 24–32px mobile
  sans 600
  -0.02em tracking
  1.1–1.2 line-height

section label
  12px
  mono 500
  0.08em tracking
  uppercase
  “00 / ABSTRACT”

body
  16–18px desktop / 15–17px mobile
  sans 400–500
  1.7–1.85 line-height
  760px max

caption and table label
  10–12px
  mono
  1.5 line-height

equation
  22–34px desktop / 18–24px mobile
  serif or math
```

Rules:

- no oversized marketing headlines
- no gradient type
- no expressive display type competing with the monument
- use tracking only for mono navigation, labels, and stamps
- use whitespace rather than extreme type scale for hierarchy
- avoid normal text below 10px
- body copy must not use `quiet-white`

## Layout

### Spacing Scale

```text
4  8  12  16  24  32  48  72  96  128  192  256
```

Use large spacing deliberately. Empty space must separate ideas, not conceal missing content.

### Widths

```text
narrow theorem   560px
longform         760px
diagram field    980px
operational UI   1180px
full field       100vw
```

### Breakpoints

```text
compact phone    <= 460px
mobile/tablet    <= 760px
wide layout      >= 1024px
```

Use content-driven adjustments between these breakpoints when a table, equation, or diagram requires them.

### Top-Level Grid

Prefer:

- one centered reading column
- occasional centered diagram field
- strong vertical sequence
- hairlines only when they clarify structure

Avoid on top-level narrative pages:

- marketing card grids
- decorative sidebars
- multi-column feature sections
- sticky promotional UI

Operational pages may be denser, but density must correspond to evidence or control.

## Navigation and Interaction

Desktop:

```text
left: everyday gold mark
center: page links
right: optional external or operational entry
```

Mobile:

```text
left: everyday gold mark
right: MENU
```

Rules:

- keep navigation visually quiet
- current page: `ink-white` plus 1px underline or equivalent
- hover: move from `soft-white` to `ink-white`; no gold
- focus: 2px `ink-white` outline with at least 4px offset
- use `aria-current="page"` for the current destination
- interactive targets should be at least 44×44px, using padding around small type
- never remove focus indication
- do not rely on color alone for active, valid, failed, or selected states

## Motion

Motion should feel like a proof resolving.

Tokens:

```text
micro feedback     120ms ease-out
standard UI        180ms ease-out
content reveal     600ms cubic-bezier(0.22, 1, 0.36, 1)
diagram draw       900ms cubic-bezier(0.22, 1, 0.36, 1)
monument drift     12s minimum, subtle, optional
```

Allowed:

- restrained opacity reveal
- small spatial settling
- diagram lines appearing in causal order
- gold appearing after white structure resolves

Avoid:

- constant fast rotation
- particle storms
- bouncy motion
- animated gradients
- parallax spectacle
- movement required to understand content

Under `prefers-reduced-motion: reduce`:

- disable looping monument motion
- make reveal content immediately visible
- preserve the final state of diagrams
- reduce transitions to effectively instant

## Landing Viewport

Required:

1. tiny navigation
2. full-spectrum monument
3. one theorem line
4. optional proof sequence

Desktop:

```text
top: navigation
center: monument
below: The alignment layer for open intelligence.
lower field: Diverge. Evaluate. Align. Resolve. Inherit. Reopen.
```

Mobile:

```text
top: mark / menu
center: monument
below: theorem
lower: shortened sequence if space requires
```

Rules:

- the still image must be complete without animation
- no hero paragraph
- no primary CTA button
- no feature cards
- no partner strip
- no decorative background
- no more than two lines of theorem copy

## Longform

Structure pages as blackpaper documents:

```text
title block
96–128px gap
00 / ABSTRACT
paragraph group
96–128px gap
figure or equation
96–128px gap
01 / SECTION
paragraph group
```

Use:

- narrow reading column
- substantial but readable paragraphs
- two to four paragraphs per conceptual block
- centered equations and figures
- small mono captions
- explicit mechanism before poetic closure

Every rationale must include:

- incentive versus alignment
- a bounded definition of alignment
- the problem of non-cumulative intelligence
- the canonical sequence
- one worked proof example
- one inherited/reopened conclusion

## Diagram Language

Primitive meanings:

```text
candidate
  faint white point, row, or line

evaluation
  axis, threshold, matrix, baseline, or bracket

invalid / regressive
  error-red plus shape, label, or strike

alignment
  shared boundary or simultaneous condition

resolution
  one path becomes clearer white

inheritance
  gold line, point, baseline, or lineage

reopening
  new faint candidates extending from inherited gold
```

Rules:

- thin strokes
- more empty space than ink
- labels are mandatory when meaning is not self-evident
- gold only marks the inherited or validated element
- failure never relies on red alone
- no generic network clouds
- no meaningless equations
- no 3D unless depth expresses a real variable

### Canonical Mechanism Figure

Show:

```text
candidate inputs
-> shared environment matrix
-> validity and non-regression test
-> resolved challenger
-> gold inherited baseline
-> reopened candidates
```

Caption:

> FIG. 01 / A valid challenger is inherited only after it clears the shared environment set.

Canonical rule:

```text
inherit(K) iff
  valid(K)
  and every required score is non-regressive
  and at least one required score improves
```

This is the Doctrine's simplified illustrative rule, not the production acceptance logic. Production comparison is statistical; see the Doctrine's Canonical Proof Example.

The figure should make simultaneous evaluation visible. Do not reduce the mechanism to an unexplained funnel or glowing node.

## Components

### Narrative Components

**Theorem block**

- centered
- no border by default
- 680px max
- large vertical margin

**Proof row**

- thin top hairline
- two columns on wide screens, one on mobile
- mono label plus explanatory text
- validation gold only on earned state

**Figure insert**

- centered
- caption below
- figure number aligned consistently
- alternative description in markup

**Alignment index**

```text
00 DIVERGE
01 EVALUATE
02 ALIGN
03 RESOLVE
04 INHERIT
05 REOPEN
```

### Operational Components

Operational surfaces may use tables, controls, status rows, and compact charts.

**Tables**

- row and column headers must be explicit
- maintain 4.5:1 text contrast
- use tabular numerals
- allow horizontal scrolling on narrow screens
- keep headers visible when useful
- use icons or labels alongside delta color
- highlight an inherited row with a gold rule or marker, not a full gold wash

**Charts**

- label axes and environments
- provide exact values when decisions depend on them
- champion and challenger must remain distinguishable without color
- reserve gold for inherited state
- use red and green only with arrows, signs, or labels
- include an accessible summary or data table

**The generational record — Affine Dashboard pattern**

This is a product-surface pattern specific to the Affine Dashboard's Evolution
chart, recorded so the implementation stays canonical. It is not a general
charting rule. Its encoding is fixed:

- hollow outline: the inherited level, carried from the replaced champion
- solid fill: what the generation earned — the delta and only the delta
- a generation that earned nothing is entirely hollow; that is information, not a gap
- `validation-gold`: the current champion generation and its earned deltas
- `gold-muted`: historical earned deltas
- value labels in `ink-white`; ties as a dim dash, never a zero
- an append-only horizontal strip, chronological left to right, scrolled to the current champion on load, scrolling inside its own region
- nearby tables carry the exact figures, satisfying the accessible-equivalent rule

**Forms and controls**

- use visible labels, not placeholder-only fields
- minimum 44px target height
- white focus state
- errors use `error-red` plus message and icon
- primary actions use white structure by default, not gold fill
- dangerous actions require explicit confirmation

**Status**

- state precedes explanation
- validated, failed, pending, and inherited states need text labels
- do not use pill badges unless compact status density truly requires them

## Accessibility Requirements

These are release requirements, not suggestions.

- normal text: minimum 4.5:1 contrast
- large text and essential non-text graphics: minimum 3:1
- body text: `muted-white` or brighter; prefer `soft-white`
- `quiet-white` is the dimmest permitted normal text token
- no opacity-based body text
- links and current states need a non-color indicator
- focus is always visible
- all interactive targets are at least 44×44px where practical
- diagrams have captions and alternative descriptions
- charts have a text or tabular equivalent
- headings follow a logical hierarchy
- modal surfaces, including the mobile menu, contain focus, render the background inert, and restore focus on close
- content remains understandable with CSS animation disabled
- validation, failure, and improvement never rely on color alone

## Mobile Rules

- preserve the monument and theorem hierarchy
- use at least 24px side padding for longform where viewport permits
- stack proof rows and component comparisons
- keep section labels small and mono
- allow tables and wide equations to scroll inside labeled regions
- simplify diagrams without deleting causal stages
- never replace the system with generic cards
- prevent the fixed navigation from covering the first heading
- test at 375×667 and 390×844 minimum

## Page Blueprints

### Home

1. monument and theorem
2. category contrast
3. canonical sequence
4. one mechanism figure
5. restrained footer

### Rationale

1. abstract
2. production without continuity
3. bounded definition of alignment
4. evaluation pressure
5. canonical proof example
6. inheritance and reopening

### Mechanism / Dashboard

1. current baseline
2. candidate field
3. required environments
4. validity and regression conditions
5. resolution decision
6. inherited lineage
7. reopened frontier

### Design System

1. governing principle
2. identity hierarchy
3. palette and contrast
4. type and layout
5. diagram and proof rules
6. components and operational patterns
7. interaction and motion
8. accessibility
9. exception governance
10. kill criteria

## First-Pass Deliverables

1. `00 Reference / 2026-06-18`
2. `01 Home / Desktop`
3. `02 Home / Mobile`
4. `03 Rationale / Desktop`
5. `04 Rationale / Mobile`
6. `05 Mechanism / Desktop`
7. `06 Operational Proof`
8. `07 Design System / Tokens`
9. `08 Diagram Primitives`
10. `09 Accessibility States`
11. `99 Review / Scoring`

Begin with the first viewport, longform rhythm, and canonical mechanism figure. Build components from those needs.

## Exception Governance

An exception is allowed only when:

1. the existing rule prevents the mechanism or interaction from being understood
2. accessibility requires a stronger treatment
3. operational density has a documented need
4. the change can be stated as a reusable rule

Record:

- the rule being overridden
- the use case
- the smallest necessary exception
- accessibility impact
- whether the Doctrine or Visual System needs updating

Do not create exceptions for novelty, decorative preference, or implementation convenience.

## Review Rubric

Score each category 0, 1, or 2.

1. **Category clarity** — alignment is immediately understood.
2. **Mechanism proof** — evaluation, resolution, inheritance, and reopening are visible.
3. **Independence** — Affine feels related to Bittensor without cloning it.
4. **Identity discipline** — monument, mark, and Lambda have distinct roles.
5. **Color semantics** — spectrum is contained and every non-brand gold state is earned.
6. **Plainness** — sparse but not underdesigned or empty.
7. **Longform authority** — reads as a blackpaper rather than marketing.
8. **Operational rigor** — claims are supported by inspectable state.
9. **Accessibility** — contrast, focus, motion, labels, and alternatives pass.
10. **Mobile integrity** — the direction survives narrow viewports.

Interpretation:

- 0–11: not the direction
- 12–15: useful exploration
- 16–18: strong candidate
- 19–20: release candidate

A release candidate must score 2 in category clarity, mechanism proof, color semantics, and accessibility.

## Kill Criteria

Reject the design if:

- it looks like generic dark-mode AI
- it reads as luxury crypto
- the spectral monument becomes a decorative palette
- gold marks generic UI instead of identity or earned state
- current navigation is gold
- diagrams are visually complex but causally empty
- small gray text falls below contrast requirements
- motion is required for comprehension
- the mechanism is replaced by mystical language
- operational density has no decision-making purpose

The landing page should be so plain that it feels brave.

The deeper pages should be so concrete that the plainness feels earned.
