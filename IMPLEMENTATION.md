# Implementation guidance

## Authority and interpretation

`BRAND_SYSTEM.md` is the full source of truth. JSON and CSS translate its explicit values. If they ever diverge, correct the derived files to match the specification. Keep suggested ranges and approximate values labeled as such.

The CSS exports minimum/maximum endpoints without choosing a global size or inventing a fluid interpolation. Hero and body line heights have supplied ranges; other line heights remain unspecified. Components use only explicit values, and button font size remains a range for the consuming project to choose from.

No breakpoints, responsive type sizes, layout widths, spacing system, icon stroke width, animation timings, disabled/error/success treatments, or numeric logo clear space are defined. Choose these per application and identify them as implementation decisions, not locked brand tokens.

## Applying the palette

Soft Ivory is the default canvas; Champagne is the secondary surface. Keep Taupe selective. Use Charcoal for body text and Ink Blue for structural emphasis. Aubergine remains a detail. The deeper navy is primarily for logos and the specified primary-button hover.

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
