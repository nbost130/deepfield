# Deepfield

A dark, sci-fi editorial theme for [Obsidian](https://obsidian.md). Named for the Hubble Deep Field.

Sparse typography. Blue glow. Technical precision. Inspired by the visual language of space documentary filmmaking.

![Deepfield Theme Screenshot](screenshot.png)

---

## Features

- **20 color palettes** switchable via the [Style Settings](https://github.com/mgmeyers/obsidian-style-settings) plugin — including 8 planet themes derived from real spectral/reflectance data
- **Dark mode only** — purpose-built for long reading sessions
- **Two-font system** — Inter for body and headings, Space Mono for section headers (uppercase, tracked)
- **Square geometry** — no border radius anywhere; tags, code blocks, and callouts all use hard corners
- **HUD-inspired components** — optional `deepfield-components.css` snippet adds custom UI elements: attribution blocks, LED indicators, progress bars, corner brackets, scan-line dividers, and more
- Compatible with [Minimal](https://github.com/kepano/obsidian-minimal) — overrides its HSL base system for full cascade

---

## Installation

### Via Community Themes (recommended)

1. Open Obsidian → Settings → Appearance → Themes → Browse
2. Search for **Deepfield**
3. Install and select

### Manual

1. Download this repo
2. Copy the `Deepfield/` folder to your vault's `.obsidian/themes/` directory
3. In Obsidian: Settings → Appearance → Themes → select Deepfield

---

## Color Palettes

Requires the [Style Settings](https://github.com/mgmeyers/obsidian-style-settings) plugin.

Once installed, go to **Settings → Style Settings → Deepfield → Color Palette**.

| Category | Palettes |
|----------|----------|
| **Blues** | Electric (default), Steel, Slate, Midnight |
| **Planets (spectral)** | Mercury, Venus, Earth, Mars, Jupiter, Saturn, Uranus, Neptune |
| **Space palettes** | Event Horizon, Galactic Noir, Midnight Orbit, Ion Trail, Aurora Nebula, Magnetic Field, Retro Galaxy, Vintage Cosmos |

The 8 planet themes are derived from real astronomical spectral data — each accent color reflects the dominant wavelength of light that planet actually reflects.

---

## Custom Components (CSS Snippet)

Copy `deepfield-components.css` to your vault's `.obsidian/snippets/` folder and enable it in **Settings → Appearance → CSS Snippets**.

This snippet adds custom HTML elements you can use in your notes:

```html
<!-- Attribution block -->
<div class="deepfield-attribution">
  <div class="deepfield-attribution-meta">Proof · Cambridge · 1974</div>
  <div class="deepfield-attribution-name">Stephen Hawking</div>
  <div class="deepfield-attribution-desc">Every black hole leaks energy. Slowly · Unstoppably</div>
</div>

<!-- HUD panel -->
<div class="deepfield-hud">
  <div class="deepfield-hud-bar"></div>
  <div class="deepfield-hud-body">Content here</div>
</div>

<!-- Punchline -->
<div class="deepfield-punchline">Slowly · Unstoppably</div>

<!-- LED status -->
<span class="deepfield-led on"></span> Confirmed
<span class="deepfield-led warn"></span> Uncertain
<span class="deepfield-led"></span> Unobserved

<!-- Progress bar -->
<div class="deepfield-bar">
  <div class="deepfield-bar-label"><span>Progress</span><span>4 / 7</span></div>
  <div class="deepfield-bar-track"><div class="deepfield-bar-fill" style="width:57%"></div></div>
</div>
```

---

## Attribution

**Visual aesthetic** inspired by [Caelum](https://www.youtube.com/@caelum) — specifically the video *The 7 Levels of Black Holes*. The dark editorial typography, monospace section headers, dot separators, and data-annotation style are drawn directly from their visual language.

**Space color palettes** sourced from [Filmora's Space Color Palette guide](https://filmora.wondershare.com/video-creative-tips/space-color-palette.html).

**Planet color palettes** derived from published spectral/reflectance data:
- Mercury: silicate surface reflectance, peak ~500nm
- Venus: sulfuric acid cloud albedo, UV absorber at 340nm
- Earth: Rayleigh scattering, ocean blue dominant at ~450nm
- Mars: ferric iron (Fe₂O₃/hematite), reflectance peak ~750nm
- Jupiter: red chromophore absorption 300–500nm
- Saturn: ammonia ice reflectance peak 550–600nm
- Uranus: methane absorption 700–900nm, reflects ~480nm
- Neptune: stronger methane than Uranus, only ~440nm escapes

**Style Settings integration** follows patterns from [mgmeyers/obsidian-style-settings](https://github.com/mgmeyers/obsidian-style-settings) and [kepano/obsidian-minimal](https://github.com/kepano/obsidian-minimal).

**CSS snippet distribution pattern** inspired by Nick Milo's [ITS Theme](https://github.com/SlRvb/Obsidian--ITS-Theme) approach.

---

## License

MIT — see [LICENSE](LICENSE)
