# Dynamic Slideshow Banner

*Mafatlal MedFits — custom section, built July 2026*

![Dynamic slideshow banner on mobile](./desktop.PNG)
![Dynamic slideshow banner on desktop](./mobile.PNG)

## What it is
A fully responsive slideshow/hero banner that shows **separate images for
desktop and mobile** per slide. Dawn's default slideshow section only
supports a single image per slide across all breakpoints — this was
custom built to add independent desktop/mobile image fields.

## Key features
- Per-slide **desktop image** and optional **mobile image** fields — if
  no mobile image is set, the desktop image is used as a fallback.
- Auto-rotate (optional) with adjustable speed, or manual prev/next
  navigation.
- Slider visual style options: dots, counter, or numbers.
- Adapts slide height to the image's aspect ratio, or fixed
  small/medium/large heights.
- Per-slide heading, subheading, button, text alignment (desktop +
  mobile separately), box position, color scheme, and image overlay
  opacity — all configurable via the theme editor.
- Full-slide clickable link overlay per slide.
- Up to 5 slides per section.

## Tech
Shopify Liquid (section + schema), responsive `<img>` with `srcset`/`sizes`, CSS, vanilla JavaScript (native slideshow component)

## Setup
Add `dynamic-slideshow-banner.liquid` to the theme's `sections/`
folder — it registers as "Dynamic Slideshow Banner" in the theme
editor's section picker. Add it to any template, then add slide blocks
and set a desktop image (required) and mobile image (optional) per
slide.

## Files
- [`dynamic-slideshow-banner.liquid`](./dynamic-slideshow-banner.liquid) — full section code