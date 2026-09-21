# Assets included and still needed

## Included PNGs

All four user-supplied PNGs are included unchanged apart from filenames. Each canvas is 3000 × 1400 pixels with transparency. Dominant fully opaque pixels match the specified navy or ivory. Source filenames, visible bounds, and SHA-256 checksums are recorded in [logos/asset-manifest.json](logos/asset-manifest.json).

| Supplied filename | Repository destination | Use |
| --- | --- | --- |
| LOFT wordmark png.png | `logos/png/loft-advisory-navy.png` | Full lockup on light backgrounds |
| LOFT wordmark ivory png.png | `logos/png/loft-advisory-ivory.png` | Full lockup on dark backgrounds |
| LOFT word only png.png | `logos/png/loft-wordmark-navy.png` | Responsive LOFT-only mark on light backgrounds |
| LOFT word only ivory.png | `logos/png/loft-wordmark-ivory.png` | Responsive LOFT-only mark on dark backgrounds |

The PNGs include substantial transparent canvas margins; CSS image dimensions describe the whole canvas, not just the visible lettering. Preserve the supplied originals. Judge legibility using the actual visible mark, especially ADVISORY. No minimum display size or cropping standard has been approved.

## Add approved SVG exports

Drop the four genuine vector exports at these paths:

- `logos/svg/loft-advisory-navy.svg`
- `logos/svg/loft-advisory-ivory.svg`
- `logos/svg/loft-wordmark-navy.svg`
- `logos/svg/loft-wordmark-ivory.svg`

Export from the approved design source. Preserve the asymmetric lockup, proportions, and artwork. Use Deep Logo Navy `#24384A` or Soft Ivory `#F7F3EC`. A PNG wrapped inside an SVG is not a vector export. Do not trace or recreate the logo from Lora.

## Add vector print masters

Place original editable vector source files or professional vector print exports in `logos/masters/`, preserving their actual file extensions. Suggested descriptive stems: `loft-advisory-master` and `loft-wordmark-master`. Do not invent CMYK, Pantone, or foil specifications; confirm production requirements with the printer.

## Fonts

No font binaries are included. Follow [font guidance](fonts-or-font-guidance/README.md) for Lora Regular (400), DM Sans Regular (400), and DM Sans Medium (500). If self-hosting, add the genuine licensed files and their supplied license notices in that directory or the application's established font directory.

## When updating assets

Use these same canonical filenames for replacement exports. Update the manifest to reflect the new files, their original filenames and checksums. Check the full and responsive variants on appropriate light/dark backgrounds at the actual deployment sizes. Switch to the LOFT-only mark when ADVISORY cannot remain legible; no universal breakpoint is specified.
