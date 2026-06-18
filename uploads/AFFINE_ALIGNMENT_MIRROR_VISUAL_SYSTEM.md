# Affine Alignment Mirror Visual System

## Purpose

This document defines the production design system for the Affine Alignment Mirror direction.

It is standalone. A designer should be able to use this document without access to the current Affine project, earlier design files, or internal notes. It contains the visual rules, page structures, typography, color, spacing, diagram language, components, mobile rules, and review criteria needed to design a new Affine site from scratch.

Companion doctrine:

`AFFINE_ALIGNMENT_MIRROR_DOCTRINE.md`

The doctrine defines meaning. This document defines rendering.

## Design Summary

Affine should look like the color-inverted counterpart to the official Bittensor website.

This is the internal design logic, not the public headline. Publicly, Affine should lead as:

> The alignment layer for open intelligence.

The Bittensor relationship should be felt through restraint, inversion, spacing, and protocol-paper rhythm. It should be stated only when the contrast helps the user understand Affine faster.

The reference aesthetic is:

- white ground
- black type
- tiny centered navigation
- large negative space
- central symbolic object
- academic longform pages
- narrow reading columns
- numbered sections
- equations and diagrams as primary visual moments
- almost no decorative color

Affine inverts that world:

- black ground
- white type
- tiny centered navigation
- large negative space
- central Affine mark
- blackpaper longform pages
- narrow reading columns
- numbered alignment sections
- equations and diagrams as proof moments
- gold only for validation and inheritance

The governing sentence:

> Black paper. White theorem. Gold validation.

## Designer Deliverables

The first design pass should include these frames:

1. `00 Reference / Bittensor Mirror Notes`
2. `01 Home / Desktop`
3. `02 Home / Mobile`
4. `03 Rationale / Desktop`
5. `04 Rationale / Mobile`
6. `05 Mechanism / Desktop`
7. `06 Design System / Tokens`
8. `07 Diagram Primitives`
9. `08 LOGOS Relationship / Optional`
10. `99 Review / Scoring`

The design file should include a short annotation on the first frame:

```text
Affine mirrors Bittensor's restraint, centered protocol composition, longform paper rhythm, and tiny navigation.
Affine departs through blackpaper atmosphere, gold validation, alignment semantics, inheritance diagrams, and the Affine mark.
```

Do not begin with a large component library. Begin with the first viewport, the longform page rhythm, and the mechanism diagram. Components should emerge from those.

## Inversion Mapping

Use this table when translating Bittensor's visual grammar into Affine.

| Bittensor reference | Affine inversion | Meaning |
| --- | --- | --- |
| white background | black background | blackpaper field |
| black text | white text | theorem / proof |
| tau mark | Lambda micro mark / full Affine mark | alignment symbol |
| network object | alignment mark / mechanism diagram | judgment and inheritance |
| incentive language | alignment language | survival, validation, composition |
| monochrome rigor | monochrome plus rare gold | validation has been earned |
| longform whitepaper | longform blackpaper | protocol thesis inverted |
| equations | equations / matrices / thresholds | mechanism proof |
| silence | silence | authority through restraint |

This is the core translation. Do not add decorative layers to make the inversion more obvious.

## Mark System

Affine has a two-level mark system.

### Micro Mark

Use `Λ` as the small Affine mark.

Purpose:

- favicon
- small nav
- mobile header
- social avatar
- document stamp
- compact footer
- tiny loading state
- protocol shorthand

The Lambda mark is Affine's answer to Bittensor's tau mark.

It should feel mathematical, minimal, and protocol-native.

Rendering:

```text
glyph: Λ
primary color: gold-validation or ink-white
minimum digital size: 16px
preferred nav size: 18px to 24px
weight: optically medium/heavy
alignment: centered on visual cap height
```

Production note:

The first prototype may use a high-quality type glyph. Final production should use an optically tuned custom Lambda derived from the Affine mark's geometry, not a random font glyph.

Do not:

- put Lambda in a circle by default
- add glow
- add gradients
- stylize it into a luxury monogram
- use it as a decorative repeating pattern
- make it compete with the full mark on large screens

### Monument Mark

Use `affine-mark-clean.png` for large identity moments.

Expected properties:

- square PNG
- transparent background preferred
- gold Affine mark
- should be used as the central first-viewport symbol

If the mark is unavailable, stop and obtain it. Do not approximate the mark with text, CSS, SVG recreation, or placeholder geometry.

The monument mark is not decorative. It is the protocol symbol at full force.

Use it for:

- landing page center
- large identity moments
- manifesto openers
- launch visuals
- full-page poster treatments
- derived geometry and styles

The rule:

```text
small sizes: Lambda
large sizes: affine-mark-clean.png and styles derived from it
```

Do not use the full mark so small that it loses detail. Do not use raw Lambda so large that the identity feels unfinished.

## Palette

The palette must be nearly monochrome.

### Core Tokens

```text
paper-black       #050505
void-black        #000000
ink-white         #F5F2EA
paper-white       #FFFFFF
soft-white        #D8D4C8
muted-white       #9B968B
faint-white       rgba(255,255,255,0.18)
hairline-white    rgba(255,255,255,0.10)
gold-validation   #D6B85A
gold-muted        #8F7832
gold-faint        rgba(214,184,90,0.20)
error-red         #B84A3A
info-blue         #7C9AB8
```

### Usage

Black:

- page background
- spatial field
- longform paper surface
- default void around content

White:

- primary text
- diagrams
- nav
- equations
- hairline structure

Gold:

- Affine mark
- validated result
- inherited frontier
- selected theorem
- replacement event
- proof marker

Red:

- failure
- invalidated state
- rejected path

Blue:

- optional informational state
- never dominant
- never used as generic AI glow

### Gold Rule

Gold must be earned.

Use gold only when the design is marking:

- validation
- inheritance
- selection
- replacement
- frontier state
- Affine mark

Do not use gold for:

- hover decoration
- generic buttons
- section dividers
- background glow
- decorative borders
- luxury mood

## Typography

The type system should match the spirit and metrics of Bittensor's site as closely as possible: small, sparse, protocol-like, and academic.

As of this handoff, Bittensor's live CSS declares these font families:

```text
Haffer
HafferSQ
TTCommonsPro
FiraCode
DM Mono
```

Use those families where licensing and technical constraints allow. Do not assume they are freely reusable in production without checking licensing.

Recommended Affine stack:

```text
Body / headings: Haffer, HafferSQ, Helvetica Neue, Arial, sans-serif
Mono labels: FiraCode, DM Mono, TTCommonsPro, SFMono-Regular, Menlo, Consolas, monospace
Equations: KaTeX_Main, STIX Two Text, Times New Roman, serif
```

If the Bittensor fonts are unavailable, use this fallback:

```text
Body / headings: Inter, Helvetica Neue, Arial, sans-serif
Mono labels: IBM Plex Mono, SFMono-Regular, Menlo, Consolas, monospace
Equations: STIX Two Text, Times New Roman, serif
```

Designer note:

The first Affine visual pass should try the Bittensor-declared stack first. Only fall back if licensing, rendering, or availability makes that impractical.

### Type Roles

Navigation:

```text
font: mono
size desktop: 11px
size mobile: 10px
weight: 600
letter spacing: 0.08em
case: uppercase
```

Hero theorem:

```text
font: sans or mono depending composition
size desktop: 15px to 20px
size mobile: 13px to 16px
weight: 500
line height: 1.5
max width: 560px
```

Page title:

```text
font: sans
size desktop: 22px to 32px
size mobile: 20px to 26px
weight: 600
line height: 1.2
```

Section label:

```text
font: mono
size: 12px
weight: 500
letter spacing: 0.08em
case: uppercase
format: 00 / ABSTRACT
```

Body:

```text
font: sans
size desktop: 15px to 17px
size mobile: 14px to 16px
line height: 1.75
weight: 500
max width: 760px
```

Captions:

```text
font: mono
size: 10px to 12px
line height: 1.5
color: muted-white
```

Equation:

```text
font: serif/math
size desktop: 22px to 34px
size mobile: 18px to 24px
color: ink-white
```

### Typography Rules

- Do not use huge marketing headlines.
- Do not use display gradients.
- Do not use expressive type unless the Affine mark is the expression.
- Keep letter spacing at 0 except mono nav and section labels.
- Let scale come from whitespace, not enormous text.
- Use centered type sparingly and deliberately.
- Body copy should read like a paper, not a landing page.

## Layout System

The layout should be almost painfully sparse.

### Page Shell

```text
min-height: 100vh
background: paper-black
color: ink-white
top nav: fixed or absolute, very small
main content: centered
```

### Spacing Scale

```text
4
8
12
16
24
32
48
72
96
128
192
256
```

Use large spacing often.

The design should not fear empty space.

### Reading Widths

Longform:

```text
max-width: 760px
```

Narrow theorem:

```text
max-width: 560px
```

Diagram field:

```text
max-width: 980px
```

Full black field:

```text
width: 100vw
min-height: 100vh
```

### Grid

Top-level pages should feel centered, not dashboard-like.

Use:

- single centered column
- occasional centered diagram field
- large vertical gaps between sections
- hairline separators only when structure requires them

Avoid:

- card grids on top-level pages
- multi-column marketing sections
- dense dashboard layouts on the landing page
- sticky sidebars
- decorative section bands

## Navigation

Navigation should be tiny and protocol-like.

Desktop:

```text
left: Lambda micro mark
center: ABOUT / RATIONALE / MECHANISM / LOGOS / DOCS
right: optional external link
```

Mobile:

```text
top left: Lambda micro mark
top right: MENU
menu opens as a sparse full-screen blackpaper list
```

Rules:

- nav should not dominate the page
- nav labels should be mono uppercase
- nav should have no filled buttons
- current page may use muted gold only if the page is validated/selected
- do not add pill buttons or SaaS CTA buttons

## Landing Page

The landing page is the most important expression.

It should feel like the inverse of Bittensor's first viewport:

```text
black field
tiny nav
centered Affine mark
single theorem line
no cards
no feature list
no gradient
no explanatory block
```

### Required Elements

1. Tiny nav.
2. Centered `affine-mark-clean.png`.
3. One thesis line.
4. Optional tiny footer proof line.

Recommended thesis:

> The alignment layer for open intelligence.

Alternate:

> Incentives produce intelligence. Alignment decides what survives.

Footer proof line:

> Evaluate. Align. Compose. Inherit. Reopen.

### Mark Treatment

Desktop:

```text
size: 180px to 260px
placement: optical center
opacity: 1
```

Mobile:

```text
size: 120px to 180px
placement: optical center
```

Do not:

- add glow
- rotate randomly
- add particle effects
- surround with decorative rings
- animate constantly

If motion is used, it should be nearly imperceptible: a slow reveal, not a performance.

## Golden First Viewport

The first viewport must be understandable as a still image.

Desktop structure:

```text
top left: Lambda micro mark
top center: ABOUT / RATIONALE / MECHANISM / LOGOS / DOCS
top right: optional WHITEPAPER or ENTER LOGOS

center:
  affine-mark-clean.png

below center:
  The alignment layer
  for open intelligence.

bottom center or lower field:
  Evaluate. Align. Compose. Inherit. Reopen.
  Optional: Bittensor is incentive. Affine is alignment.
```

Mobile structure:

```text
top left: Lambda micro mark
top right: MENU

center:
  affine-mark-clean.png

below center:
  The alignment layer
  for open intelligence.

lower:
  Evaluate. Inherit. Reopen.
```

First viewport rules:

- no cards
- no hero paragraph
- no primary CTA button
- no social proof strip
- no partner logos
- no animated background
- no explanatory diagram unless the mark itself is the diagram
- no more than two lines of thesis copy

The opening must feel almost empty. That emptiness is the claim.

If the first viewport feels "safe" in a conventional startup sense, it is probably not brave enough.

## Longform Pages

Longform pages should feel like blackpaper sections.

Use:

- centered title
- author or source line if needed
- section labels like `00 / ABSTRACT`
- generous vertical rhythm
- narrow text column
- centered diagrams/equations
- small figure numbers at right

### Example Structure

```text
AFFINE: THE ALIGNMENT LAYER

00 / ABSTRACT

Distributed intelligence can produce capability without producing continuity...

01 / INCENTIVE

Bittensor creates market pressure...

02 / ALIGNMENT

Affine defines the conditions under which useful intelligence is retained...
```

### Body Rules

- Keep paragraphs substantial but not dense.
- Use large gaps between conceptual blocks.
- Avoid cards and callout boxes.
- Equations should sit alone with breathing room.
- Diagrams should be centered and quiet.
- Gold may identify the resolved or inherited part of a diagram.

### Longform Rhythm

Use this approximate rhythm on rationale and manifesto pages:

```text
title block
128px gap
00 / ABSTRACT
body paragraph group
128px gap
figure or equation
128px gap
01 / SECTION
body paragraph group
```

The longform page should feel slow in a good way. The user should feel that each section is being placed, not streamed.

Paragraph groups should usually contain two to four paragraphs. Do not create dense essay walls.

### Longform Content Requirements

Every rationale page must include:

- the incentive/alignment distinction
- the problem of non-cumulative intelligence
- the Affine mechanism sequence
- one diagram or equation
- one gold validation/inheritance moment
- a closing statement that reopens the frontier

If the page only argues philosophically and never shows mechanism, it is incomplete.

## Diagram Language

Diagrams are essential.

They should be sparse, mathematical, and explanatory.

### Diagram Primitives

Candidate:

```text
thin white point, line, or row
```

Evaluation pressure:

```text
axis, threshold, bracket, matrix, baseline
```

Alignment:

```text
parallel convergence, shared boundary, weighted relation
```

Resolution:

```text
one line or node becomes clearer
```

Inheritance:

```text
gold line, gold point, gold baseline
```

Reopening:

```text
new faint candidates after inherited state
```

### Diagram Rules

- Use thin strokes.
- Use far more empty space than ink.
- Use gold only for the selected/inherited element.
- Label diagrams with mono captions.
- Do not use 3D unless it is directly meaningful.
- Do not use decorative network clouds without explanation.
- Do not use random particles.
- Do not over-animate.

## Equation Treatment

Equations can be used as brand moments if they are meaningful.

Rules:

- center equations
- use serif/math font
- give them large vertical space
- keep labels small and mono
- number equations at the right edge when appropriate
- use gold only to mark the selected variable or validation term

Do not fake rigor with meaningless formulas.

If an equation appears, it must correspond to an actual concept on the page.

## Canonical Mechanism Diagram

Every first design pass should include one canonical Affine mechanism diagram.

It should show:

```text
candidate inputs -> evaluation pressure -> resolved path -> gold inheritance line -> reopened candidates
```

Visual requirements:

- candidates are faint white
- evaluation pressure is a thin white threshold, matrix, or axis
- resolved path is clearer white
- inherited state is gold
- reopened candidates are faint white after the gold state

Caption:

> FIG. 01 / Alignment converts evaluated output into inherited frontier.

Do not make the diagram a generic network sphere. The diagram must show selection and inheritance.

## Component Language

Most top-level pages should avoid conventional components.

When components are needed, use blackpaper components:

### Theorem Block

Purpose:

- central thesis
- compressed proof
- replacement rule

Style:

```text
no border by default
centered
max-width: 680px
large vertical margin
```

### Proof Row

Purpose:

- compare incentive and alignment
- show before/after
- show candidate/resolved states

Style:

```text
thin top hairline
two columns desktop
single column mobile
mono label
body text
gold only on validated term
```

### Figure Insert

Purpose:

- diagram or equation

Style:

```text
centered
wide spacing
caption below
figure number right aligned
```

### Alignment Index

Purpose:

- list the core sequence

Style:

```text
00 DIVERGE
01 EVALUATE
02 ALIGN
03 RESOLVE
04 INHERIT
05 REOPEN
```

Current or inherited stage may use gold.

### Validation Marker

Purpose:

- mark inherited or validated state

Style:

```text
small gold dot, line, or mono label
never a large badge
```

Avoid:

- pill badges
- rounded cards
- big CTA buttons
- colorful chips
- heavy shadows
- glassmorphism

## Page Blueprints

### Home

Sections:

1. First viewport: mark and theorem.
2. Alignment statement: Bittensor incentive / Affine alignment.
3. Mechanism sequence: Diverge -> Evaluate -> Align -> Resolve -> Inherit -> Reopen.
4. One proof diagram.
5. Footer nav.

Keep the home page short.

### Rationale

Sections:

1. Abstract.
2. The problem of incentive without inheritance.
3. The alignment layer.
4. Evaluation pressure.
5. Replacement and inheritance.
6. Open frontier.

### Mechanism

Sections:

1. Input field: independent capabilities.
2. Evaluation matrix.
3. Alignment threshold.
4. Resolution event.
5. Inheritance baseline.
6. Reopening cycle.

### Design System

Sections:

1. Blackpaper principle.
2. Palette.
3. Type.
4. Layout.
5. Diagram primitives.
6. Gold rule.
7. Kill criteria.

### LOGOS

Sections:

1. LOGOS as operational surface.
2. Word made operational.
3. Run/loop/trace/artifact proof.
4. User controls.
5. Relationship to Affine alignment.

LOGOS may be denser than Affine pages, but it should still use the blackpaper restraint.

## Mobile Rules

Mobile must preserve plainness.

Rules:

- nav collapses to Lambda micro mark + menu
- mark remains central on home
- theorem line should not wrap into awkward fragments
- longform text gets generous side padding: 24px minimum
- equations may scale down but must remain readable
- diagrams may become stacked or scrollable
- section labels remain mono and small
- do not replace the design with generic mobile cards

Mobile first viewport:

```text
top: Lambda micro mark / menu
center: full Affine mark
below: theorem line
bottom: optional sequence line
```

## Motion

Motion is optional and should be almost silent.

Allowed:

- slow fade in
- slight mark reveal
- diagram line drawing on scroll
- gold validation appearing after white structure
- section text entering with subtle opacity

Avoid:

- constant logo spin
- particle storms
- parallax spectacle
- animated gradients
- bouncy UI motion
- anything that makes the page feel like a launch campaign

Motion should feel like a proof resolving, not a product performing.

## Accessibility

Minimalism cannot reduce usability.

Requirements:

- maintain readable contrast between white text and black background
- body text should not be pure low-opacity gray
- gold text on black must be large or supported by shape/label
- links need visible focus states
- mobile menu must be keyboard accessible
- diagrams need captions or alternative descriptions
- avoid relying on color alone to communicate validation

## Copy Density

The system should use less copy on landing and more copy in longform.

Landing:

```text
1 theorem line
1 sequence line
optional nav
```

Longform:

```text
full paragraphs allowed
large vertical gaps required
diagrams interrupt text
```

Product / LOGOS:

```text
short operational labels
state before explanation
trace before claim
```

## Standalone Handoff Checklist

A designer receiving only this document and the doctrine should have:

- product premise
- Bittensor relationship
- visual reference logic
- palette
- typography
- layout system
- landing blueprint
- longform blueprint
- diagram rules
- component rules
- mobile rules
- review criteria

If any of these are missing from a design file, the handoff is incomplete.

## Review Checklist

Before calling a design complete, answer:

1. Does it look like a blackpaper counterpart to Bittensor?
2. Does it communicate alignment, not generic AI?
3. Is Lambda used for small-size identity and the full Affine mark used for large identity?
4. Is gold rare and meaningful?
5. Does the first viewport avoid marketing clutter?
6. Is the page mostly black, white, and silence?
7. Are diagrams or equations meaningful?
8. Does the page use whitespace as structure?
9. Does the design still work if animations are disabled?
10. Does it feel like Affine could belong in the Bittensor world without pretending to be Bittensor?

## Scoring Rubric

Score each category 0, 1, or 2.

1. **Mirror**
   0: no clear Bittensor relationship
   1: visually similar but not conceptually clear
   2: unmistakable inverted counterpart

2. **Independence**
   0: feels like a clone
   1: has some Affine cues
   2: clearly Affine through alignment, gold validation, Lambda, and full mark usage

3. **Plainness**
   0: too much marketing/UI clutter
   1: minimal but still conventional
   2: brave, sparse, protocol-like

4. **Alignment**
   0: unclear what Affine does
   1: alignment stated but not shown
   2: alignment is visible in copy and mechanism

5. **Gold Discipline**
   0: gold is decorative
   1: mostly meaningful
   2: every gold moment is earned

6. **Longform Authority**
   0: reads like marketing
   1: somewhat paper-like
   2: reads like a blackpaper/protocol artifact

7. **Diagram Proof**
   0: no mechanism diagram
   1: diagram exists but is generic
   2: diagram shows evaluation, resolution, inheritance, and reopening

8. **Typography**
   0: generic web typography
   1: close but inconsistent
   2: tiny nav, controlled hierarchy, paper-like reading rhythm

9. **Mobile**
   0: collapses into generic mobile page
   1: mostly preserves the direction
   2: keeps the blackpaper identity intact

10. **Memorability**
   0: forgettable
   1: tasteful but not iconic
   2: plainness becomes the memorable move

Score interpretation:

- 0-11: not the direction
- 12-15: useful exploration
- 16-18: strong candidate
- 19-20: 10/10 candidate

Do not call a design 10/10 unless it scores 19 or 20 and earns 2 points in Mirror, Independence, Alignment, and Gold Discipline.

## 10/10 Visual Bar

A 10/10 execution:

1. Looks nearly inevitable.
2. Feels minimal without feeling underdesigned.
3. Makes black feel like paper, not dark mode.
4. Makes white feel like theorem, not generic text.
5. Makes gold feel like validation, not decoration.
6. Makes the Affine mark feel canonical.
7. Uses Lambda as the micro signature without making the system feel like a logo swap.
8. Uses Bittensor's restraint as a mirror, not a costume.
9. Makes longform content feel worth reading.
10. Makes diagrams feel like proof.
11. Can be understood as a still image.

## Final Art Direction

Design Affine as a blackpaper protocol site.

Use the same kind of silence, restraint, centered composition, narrow reading columns, small mono navigation, and academic rigor found in Bittensor's site, but invert the palette and change the meaning.

Bittensor's world is white paper and black incentive signal.

Affine's world is black paper, white alignment theorem, and gold validated inheritance.

The landing page should be so plain that it feels brave.

The deeper pages should be so rigorous that the plainness feels earned.
