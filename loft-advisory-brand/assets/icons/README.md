# Brand icons

Original supplied PNGs, unchanged:

- `loft-icon-512.png`: 512 × 512 square icon for high-resolution square applications.
- `loft-favicon-32.png`: 32 × 32 browser favicon.

Both use an ivory L (#F7F3EC) on Ink Blue (#2B4057). The user approved this supplied color as the standard. Dimensions and hashes are recorded in [the manifest](../asset-manifest.json).

When deployed at this path, add to a site's HTML head:

```html
<link rel="icon" type="image/png" sizes="32x32" href="/assets/icons/loft-favicon-32.png">
```

Adapt the URL to the consuming site's asset convention. The 512 px icon can serve square profile/app uses; it does not by itself configure a web app manifest or Apple touch icon. No additional sizes are required for this scope.
