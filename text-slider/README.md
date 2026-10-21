# Text Slider (Dynamic Marquee)

*Mafatlal MedFits — custom section, built July 2026*

![Text slider output](./output.PNG)
![Text slider on mobile](./mobile-op.PNG)

## What it is
A fully configurable scrolling marquee/text-ticker section — used here
for product feature highlights (Pockets, Stretchable, Lightweight,
Breathable, etc.) and promotional banners. Not a default Dawn section;
built from scratch to be reusable anywhere a scrolling text strip is
needed.

## Key features
- **Seamless infinite loop** — JS calculates the exact width of one
  group of items and drives the CSS animation by that distance, so there
  are no visible gaps or restart jumps.
- Repeatable blocks per item: text, optional link (with new-tab option),
  optional icon, optional per-item text/background color override,
  optional separator (custom character per item or section default).
- Left/right scroll direction, pause-on-hover toggle.
- Independent desktop/mobile control over height, font size, item
  spacing, and scroll speed.
- Typography controls: font weight, letter spacing, text alignment.
- Accessibility: respects `prefers-reduced-motion` (falls back to a
  static, wrapped layout instead of animating), configurable
  accessibility label.
- Advanced: optional custom CSS class and custom CSS field for extra
  per-section tweaks without editing the section file.

## Tech
Shopify Liquid (section + schema), CSS (custom properties, keyframe
animation, `prefers-reduced-motion`), vanilla JavaScript (dynamic width
calculation for seamless looping)

## Setup
Add `text-slider.liquid` to the theme's `sections/` folder — it
registers as "Dynamic marquee" in the theme editor's section picker.
Add it to any template, then add "Marquee item" blocks with your text,
links, icons, and separators as needed.

## Files
- [`text-slider.liquid`](./text-slider.liquid) — full section code