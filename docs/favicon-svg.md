# `images/favicon.svg` — icon

Hand-crafted SVG favicon. 64×64 viewBox, referenced once from the
`<head>` of `index.html`:

```html
<link rel="icon" type="image/svg+xml" href="images/favicon.svg">
```

## Composition

- Rounded square background (`rx="14"`) filled with a linear gradient
  from **primary** `#008000` (top-left) to **accent** `#FFFFFF`
  (bottom-right).
- Centered capital letter — the first character of **Barbershop** —
  rendered in the system UI font at 36px, weight 800, white.

## Why SVG

- Scales perfectly at any size (16px tab icon, 512px app icon).
- Zero raster assets, so nothing to compress or export.
- Colors are inlined into the SVG — no CSS dependency.

## Retheming

Edit the two `stop-color` values in the `<defs>` block to match a new
brand palette:

```xml
<stop offset="0" stop-color="#008000"/>
<stop offset="1" stop-color="#FFFFFF"/>
```

Or change the initial by editing the `<text>` content — useful if the
site is renamed.