# Implementation guidance

## Authority and interpretation

`BRAND_SYSTEM.md` is the full source of truth. JSON and CSS translate its explicit values. If they ever diverge, correct the derived files to match the specification. Keep suggested ranges and approximate values labeled as such.

The CSS exports minimum/maximum endpoints without choosing a global size or inventing a fluid interpolation. Hero and body line heights have supplied ranges; other line heights remain unspecified. Components use only explicit values, and button font size remains a range for the consuming project to choose from.

No breakpoints, responsive type sizes, layout widths, spacing system, icon stroke width, animation timings, disabled/error/success treatments, or numeric logo clear space are defined. Choose these per application and identify them as implementation decisions, not locked brand tokens.

## Applying the palette

Soft Ivory is the default canvas; Champagne is the secondary surface. Keep Taupe selective. Use Charcoal for body text and Ink Blue for structural emphasis. Aubergine remains a detail. Logos and icon backgrounds use the user-approved Ink Blue. Deep Navy #24384A remains only as the specified primary-button hover color.

On Ink Blue or Aubergine fields, use Soft Ivory text and ivory logos. The example button, link and field classes target light surfaces; do not blindly reuse their Ink Blue text on dark fields. Adapt context deliberately and check readability in the finished interface.

## Interface behavior

The reference CSS defines primary and secondary button colors, selected backgrounds, link hover underlining and field colors/borders. Shared button font and approximate padding follow the general button guidance. It leaves browser focus outlines in place; field focus changes the outline color only. A numeric focus width/offset is not locked.

Do not remove keyboard focus indication. Verify keyboard navigation, contrast and zoom behavior in the finished application. The brand specification's thin Taupe field border is retained as given; its inclusion is not a claim of accessibility compliance in every context.

The example contains no form submission or business functionality. Use real semantic controls, labels and state attributes in the application.

## Logo integration

Prefer the actual SVG exports once supplied. Until then, use the included PNGs without CSS filters or recoloring. Keep intrinsic proportions using `height: auto` and constrain width to the layout. Transparent margins are present in the source PNG canvases and have not been cropped.

Select the full or responsive logo by visible legibility at the intended size. No automatic pixel breakpoint is invented. Use meaningful alternate text when the logo conveys identity; use empty alternative text when it is purely redundant decoration.

## Print

Retain original vector artwork and have the print provider manage production-specific color conversion. Hex colors are supplied; CMYK/Pantone equivalents, stock weights and foil codes are not specified.

## Paths and migration

Paths in this document are relative to the repository root. Use `assets/logos/png/`, `tokens/brand-tokens.json`, `tokens/tokens.css`, and `examples/reference.css`. The manifest is `assets/asset-manifest.json`; its paths are relative to `assets/`. See [icon guidance](../assets/icons/README.md) for included PNGs and favicon markup.

The former root `tokens.json` has a different schema and retired values. It is archived, not a drop-in alias. Consumers must explicitly migrate to `tokens/brand-tokens.json`. Update all old logo and document paths using [the cleanup report](CLEANUP_REPORT.md) before deploying a consuming site. External repositories were not inspected or edited.

The old CSS token `--loft-color-deep-logo-navy` is replaced by `--loft-color-deep-navy-hover` for the retained #24384A hover color. Logo and icon semantic tokens now point to Ink Blue. Do not apply color filters to the PNGs.
