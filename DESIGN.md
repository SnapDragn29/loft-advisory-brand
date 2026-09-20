# LOFT Advisory

Strategic advisory firm serving physicians and independent medical practices — helping providers build new practices, strengthen existing ones, and make informed decisions about growth, operations, finance, and long-term direction.

**The brand should feel:** serious, sophisticated, intelligent, established, highly capable — premium because of proportion, typography, and restraint rather than decorative luxury cues. LOFT is personal and relationship-driven, but warmth lives in the writing, photography, and client experience — not in the visual system's softness.

## Core visual concept

The identity draws conceptually from the name LOFT: height, elevation, architectural structure, proportion, framing, grids, verticality, negative space, perspective, strong foundations, upward movement. These ideas stay **abstract** — no literal buildings, rooftops, blueprints, floor plans, columns, skylines, or construction imagery. The goal is an architectural *point of view*, not an architecture-themed brand.

## Logo

The logo is **typographic only** — no bird, wing, monogram, crest, or unrelated icon.

**LOFT wordmark** — `display` family (Bodoni Moda), uppercase, `ink-navy`. Uses customized character spacing, not uniform tracking:
- L→O: −9%
- O→F: −15%
- F→T: −6%

The word should feel compact, tall, cohesive, architectural — the L/O close at the lower forms, O/F the tightest relationship, F/T meeting or nearly meeting along their upper horizontal structure. Don't alter the Bodoni Moda letterforms themselves; distinctiveness comes from proportion and spacing, not customization.

**ADVISORY descriptor** — `condensed` family (Avenir Next Condensed Light only), uppercase, `ink-navy`, sits beneath LOFT. Track it out until ADVISORY's full width matches LOFT's width exactly; the A aligns to LOFT's left edge, the Y to its right edge. Keep enough vertical separation that both lines stay legible while reading as one lockup. ADVISORY must stay visually secondary — never Regular, Medium, Demi Bold, or Bold.

**Configurations:** stacked (LOFT / ADVISORY) is primary; LOFT alone is secondary, for when the full name is already established or space is limited. Reverse: ivory on `ink-navy`. Monochrome: `ink-navy` on ivory preferred over true black/white.

**Clear space:** generous — roughly the width of the O in LOFT, minimum, on every side. Never crowd the wordmark with rules, photography, copy, or borders.

**Files:** the wordmark lives in the Logos asset group as both SVG (preferred — scales cleanly, use everywhere possible) and PNG (for contexts that don't accept vector), in both colorways:
- `LOFT-wordmark-navy.svg` / `.png` — Deep Navy on transparent, for use on ivory or light grounds.
- `LOFT-wordmark-ivory.svg` / `.png` — Ivory on transparent, for use on Deep Navy or dark grounds (the reverse configuration).

These are the only approved wordmark files — always use them as-is rather than recreating the mark from the spacing spec above; that spec exists to explain the construction, not to be re-derived per use.

## Color

Primary palette: `surface-ivory`, `ink-navy`, `slate-blue`, `cool-gray`, `soft-gray`, `deep-plum` (see tokens for exact hex and usage on each).

Most compositions should be **dominated by ivory and navy**. Slate and gray tones provide structure. Deep Plum should generally occupy only a small percentage of any composition — avoid large deep-plum fields unless there's a deliberate exceptional reason; it should feel like a discovery, not compete with navy as the primary color.

## Typography

- **`display` (Bodoni Moda)** — used selectively: major headlines, high-impact titles, pull quotes, large numerals, select editorial statements, the wordmark. Not for paragraphs, navigation, dense copy, forms, or tables — it stays special.
- **`body` (Avenir Next Regular)** — primary body typeface: website copy, proposals, presentations, contracts, descriptive/informational content, longer-form reading. Comfortable line spacing; never compressed.
- **`body` Medium/Demi Bold** — subheads, in-copy emphasis, functional hierarchy, table headings, important labels. Used selectively — heavy sans should never dominate the identity.
- **`condensed` (Avenir Next Condensed Light)** — eyebrow text, section identifiers, short uppercase labels, small category names, occasional navigation. Generous tracking; never for paragraph-length copy.

**Hierarchy:** major display headline → section headline (Bodoni for editorial sections, Body/functional-headline for functional ones) → body copy → subhead/emphasis → eyebrow/section label. Large numerals in Bodoni Moda are especially appropriate for the LOFT Blueprint's 01–05 sequence.

> **Font-file note:** Bodoni Moda and Raleway are both hosted Google Fonts and need no file upload. Avenir Next Pro (Regular, Demi) is officially licensed by LOFT for webfont use, but under a license restricted to the site owner's own hosting — the licensed files are never uploaded to this system or any third-party tool. `body` and `condensed` reference Avenir Next by name (so it renders correctly on the many devices — Mac, iOS — where it's already installed) and fall back to Raleway rather than Helvetica Neue/Arial where it isn't. When the actual site is built, add `@font-face` declarations there pointing at the licensed `.woff2` files hosted on LOFT's own domain — that step happens outside this design system, on infrastructure LOFT controls.

## Layout philosophy

Intentional and structurally composed: generous margins, strong alignment, tall compositions, disciplined grids, vertical and horizontal rhythm, substantial negative space, deliberate asymmetry, clean hierarchy. Whitespace creates *proportion and authority*, not just air — avoid filling every available area.

## Structural graphic language

No standalone symbol — brand recognition comes from repeated structural elements instead:
- **Thin rules** — `ink-navy`, `slate-blue`, or `cool-gray` generally; `deep-plum` occasionally, for emphasis.
- **Partial frames** — incomplete boxes, corners, framing structures rather than decorative borders. Don't enclose every content area.
- **Verticality** — tall layouts, deliberate vertical spacing; let some elements extend vertically beyond convention. Reinforces "elevation" subtly.
- **Grids** — visible or implied grid relationships; every element should feel intentionally placed. Avoid loose, floating arrangements.

## The LOFT Blueprint

01 DISCOVER · 02 DESIGN · 03 BUILD · 04 LAUNCH · 05 GROW

Numerals in `display` (Bodoni Moda); labels in `condensed` or `body` Medium depending on scale; strong alignment; thin structural rules; generous spacing. Should read as a professional advisory framework — no playful progress graphics or rounded workflow bubbles.

## Photography

**Use:** real independent medical practices, thoughtful architectural interiors, physicians working naturally, consultation/decision-making environments, refined workspace details, stone/glass/paper/wood/metal materials, calm clinical environments, subtle landscape imagery supporting perspective/direction themes. Observational, not staged. Cool-neutral, sophisticated grading.

**Avoid:** generic smiling medical teams, handshake photos, staged conference-room stock, doctors pointing at tablets, isolated stethoscopes, medical crosses, heart icons, overt wellness photography, pastel lifestyle imagery, intentionally feminine imagery, excessive greenery-for-upscale-feel, luxury clichés. LOFT is not a med spa, wellness practice, coaching business, or lifestyle consultancy.

## Iconography

Minimal geometric line icons only, when icons are necessary: precise, mature, functional, visually consistent. No bubbly, rounded, cute, illustrative, or hand-drawn icons. No medical icons unless the information genuinely requires them.

## UI & components

Avoid excessive cards — not every block needs a container. When containers are needed: `radius-none` preferred, `radius-sm` only when functionally useful; no pill shapes except where interface convention requires them; no heavy shadows; no floating rounded rectangles as a primary motif. Structure comes from spacing, alignment, rules, and typography before boxes.

**Buttons** — restrained and substantial, `radius-none` or `radius-sm`, never large rounded pills:
- Primary: `ink-navy` background, ivory text.
- Secondary: ivory background, `ink-navy` text, thin navy outline.
- `deep-plum` may appear as an occasional interaction accent — never the default CTA color.

**Data & charts** — `ink-navy` for primary information, `slate-blue` for secondary, grays for context, `deep-plum` only for purposeful emphasis. No rainbow palettes. Tables: generous spacing, thin rules.

## Tone of visual luxury

Premium without trying to look luxurious. Avoid: gold, foil effects, marble, black backgrounds as default, ornate serif type, decorative monograms, fashion-brand tropes, excessive letterspacing purely to signal luxury. Sophistication comes from the quality of composition.

## Brand personality

Experienced without being traditional. Sophisticated without being precious. Human without being soft. Authoritative without being corporate. Modern without chasing trends. Premium without being fashion-oriented.

## Things to avoid completely

Swans, birds, wings, feathers, leaves, botanical symbols, soft blush palettes, rounded wellness branding, decorative monograms, scripts, handwritten type, literal buildings, blueprints-as-imagery, architecture clichés, generic healthcare symbolism, gradients as a major device, excessive shadows, overly condensed layouts, overly delicate typography, generic tech-startup minimalism.

## The brand decision test

Before introducing a visual element, ask: *does this make LOFT feel more structured, elevated, credible, and substantial?* If something exists mainly to look prettier, softer, friendlier, or more decorative, reconsider it.

## Tagline status

No finalized tagline. "Strategy for a stronger tomorrow." is under consideration and may be used experimentally — not a permanent part of the logo, not assumed on every asset, not the foundation the identity is built around.

## Default environment

Ivory background, `ink-navy` typography, cool blues/grays for support, restrained `deep-plum` accents. `display` (Bodoni Moda) as the distinctive display face, `body`/`condensed` (Avenir Next system) for function. Strong proportion, height, thoughtful negative space, architectural alignment, fine rules, structured information, disciplined hierarchy — appropriate for a sophisticated advisory firm trusted by physician owners with consequential business decisions. Never a wellness brand, boutique coaching business, fashion label, generic consulting company, or healthcare corporation.
