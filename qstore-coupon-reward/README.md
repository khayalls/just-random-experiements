# qstore-coupon-reward

The QStore "Your account is ready" screen (Qarabağ FK) built from the Figma frame `07 / 10 AZN Off` (node `1081:18437`), with a 3D hover on the coupon.

- **Live:** https://claude.ai/artifact/6HwgQxv6hAGaQfk4jJvnxg (private, use Share to open it to others)
- **Figma:** https://www.figma.com/design/xUCxbEbpflEdDmio04RFwe/Personal-Website?node-id=1081-18437

## What it tries out

- **Figma shadows.** The 5-layer soft box shadow on the white screen and the 5-layer drop shadow on the coupon, copied from Figma.
- **Fit to window.** The 1440×900 screen is scaled with `min((vw − 64) / 1440, (vh − 64) / 900)`, like Figma's zoom-to-fit, so it fills the window with a 32px margin. Below 760px wide it switches to a fluid phone layout instead of shrinking.
- **3D coupon hover.** Moving the pointer tilts the card up to 14°, lifts it, moves the light, bevel, rim highlight and cast shadow, and shifts the printed art slightly for parallax. It eases back when the pointer leaves, and stays still under `prefers-reduced-motion`.
- **Euro slot.** The hanger hole is punched through the card with a CSS mask, so the page and the card's shadow show through it, and a shaded edge gives the cut some thickness.
- **Materials.** `?material=soft` (default), `gloss` or `foil`, or `#soft` / `#gloss` / `#foil`. There is no on-screen switcher, so screen recordings stay clean.

## Run it

```bash
cd qstore-coupon-reward
python3 -m http.server 8837
```

Then open http://127.0.0.1:8837/?material=soft.

Plain HTML, CSS and JS with no build step. The font is Google Sans Flex from Google Fonts. The logo and coupon graphics in `assets/` were exported from the Figma file.
