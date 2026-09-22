# LOFT brand cleanup report

Source: https://github.com/SnapDragn29/loft-advisory-brand

Audited commit: `bbaa4750b71bfdabc4d1ed7c1a391a5df6dd9b1b`. All 24 tracked files were inspected. This is a local cleaned copy; GitHub has not been modified.

## Findings and applied changes

- Kept the four PNGs introduced by the latest “new logo files” commit as the current approved artwork, unchanged byte for byte. Renamed them consistently in assets/logos/png.
- Archived eight earlier logo exports (six PNGs, two SVGs), the conflicting DESIGN.md and tokens.json, and the superseded asset-manifest.json. No source files were discarded.
- Resolved two uppercase/lowercase PNG filename collisions by separating historical generations. Files were recovered directly from Git objects, so neither colliding version was lost.
- Updated the current brand system, JSON/CSS tokens, asset manifest, implementation and AI guidance. Fixed the example logo path and replaced broken asset/font references.
- The old tokens.json used a different schema, old palette, and Bodoni/Avenir/Raleway site typography. It is archived. Consumers must migrate explicitly to tokens/brand-tokens.json.
- No byte-identical duplicate files, mockups, photography, or placeholder images were found. No files were permanently deleted.
- “Elevating independent medicine” was not found in the source text files. The experimental “Strategy for a stronger tomorrow” appears only in the archived guide. Neither is approved current copy.
- Added both user-supplied icon exports unchanged at assets/icons/loft-icon-512.png and assets/icons/loft-favicon-32.png. Verified dimensions and colors.
- Measured new navy logos/icons as #2B4057 rather than #24384A. The user explicitly adopted the supplied Ink Blue color. Updated all active guidance and tokens accordingly; #24384A remains only as the existing functional button hover color.

## User input still needed

No requested PNGs remain missing. Current SVG/master exports are optional future inputs; existing archived SVGs are not substitutes. There are no ambiguous deletion candidates: all superseded unique files were retained. External consumers of old paths must be identified before deployment.

## Original-to-new file map

| Original path | New path | Action |
|---|---|---|
| `LOFT word only new ivory png.png` | `assets/logos/png/loft-wordmark-ivory.png` | Renamed; artwork unchanged |
| `LOFT word only new png.png` | `assets/logos/png/loft-wordmark-navy.png` | Renamed; artwork unchanged |
| `LOFT wordmark new ivory png.png` | `assets/logos/png/loft-advisory-ivory.png` | Renamed; artwork unchanged |
| `LOFT wordmark new png.png` | `assets/logos/png/loft-advisory-navy.png` | Renamed; artwork unchanged |
| `AI_HANDOFF.md` | `docs/AI_HANDOFF.md` | Updated / relocated |
| `ASSETS_NEEDED.md` | `docs/ASSETS_NEEDED.md` | Updated / relocated |
| `IMPLEMENTATION.md` | `docs/IMPLEMENTATION.md` | Updated / relocated |
| `BRAND_SYSTEM.md` | `BRAND_SYSTEM.md` | Updated / relocated |
| `README.md` | `README.md` | Updated / relocated |
| `brand-tokens.json` | `tokens/brand-tokens.json` | Updated / relocated |
| `tokens.css` | `tokens/tokens.css` | Updated / relocated |
| `components.html` | `examples/components.html` | Updated / relocated |
| `reference.css` | `examples/reference.css` | Moved unchanged |
| `DESIGN.md` | `archive/initial-brand-system/DESIGN.md` | Archived unchanged |
| `tokens.json` | `archive/initial-brand-system/tokens.json` | Archived unchanged |
| `asset-manifest.json` | `archive/previous-brand-system/asset-manifest.json` | Archived unchanged |
| `LOFT-wordmark-ivory.png` | `archive/initial-brand-system/logos/loft-wordmark-ivory.png` | Archived unchanged |
| `LOFT-wordmark-ivory.svg` | `archive/initial-brand-system/logos/loft-wordmark-ivory.svg` | Archived unchanged |
| `LOFT-wordmark-navy.png` | `archive/initial-brand-system/logos/loft-wordmark-navy.png` | Archived unchanged |
| `LOFT-wordmark-navy.svg` | `archive/initial-brand-system/logos/loft-wordmark-navy.svg` | Archived unchanged |
| `loft-advisory-ivory.png` | `archive/previous-brand-system/logos/loft-advisory-ivory.png` | Archived unchanged |
| `loft-advisory-navy.png` | `archive/previous-brand-system/logos/loft-advisory-navy.png` | Archived unchanged |
| `loft-wordmark-ivory.png` | `archive/previous-brand-system/logos/loft-wordmark-ivory.png` | Archived unchanged |
| `loft-wordmark-navy.png` | `archive/previous-brand-system/logos/loft-wordmark-navy.png` | Archived unchanged |

## Added files

Two original icon PNGs; README guidance for logos, icons, examples, and archive; docs/FONT_GUIDANCE.md; assets/asset-manifest.json; this report; docs/file-migration.json. Root README.md was rewritten.

## Upload instructions

This ZIP contains a complete replacement working tree, not a set of additions. Uploading it over the old root without removing the former paths will leave retired files mixed with current ones. Keep Git history intact: use a normal commit that adds the new folders, updates README.md and BRAND_SYSTEM.md, and removes the other old root paths listed above after confirming their replacements are present. Do not delete the repository itself. Review the change before merging and update any consuming website paths.

The accompanying Git patch applies the same changes to the audited commit and includes the binary artwork moves. The ZIP can be used without Git. GitHub itself remains unchanged until you upload/commit the result.
