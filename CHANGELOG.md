# Changelog

All notable changes to Deepfield are documented here.
Format follows [Keep a Changelog](https://keepachangelog.com/); versions follow [Semantic Versioning](https://semver.org/).

## [1.0.0] — 2026-06-06

First public release.

### Added
- **Dark + light modes.** Dark "deep space" base; light "Daylight Readout" cool-neutral paper variant. Palette accents carry into both modes.
- **20 color palettes** via the Style Settings plugin:
  - Blues — Electric (default), Steel, Slate, Midnight
  - Planets — Mercury, Venus, Earth, Mars, Jupiter, Saturn, Uranus, Neptune (accents derived from real planetary spectral/reflectance data)
  - Space — Event Horizon, Galactic Noir, Midnight Orbit, Ion Trail, Aurora Nebula, Magnetic Field, Retro Galaxy, Vintage Cosmos
- **Typography** — Inter (body, H1, H3) + Space Mono (H2, H4–H6, labels, tags, code). H2 as wide-tracked mono caps with accent rule.
- **Custom task-state glyphs** — `[x]` check, `[/]` dot (amber), `[-]` minus (faint), `[>]` arrow (purple), `[!]` triangle (red), each in its own color.
- **Tags** as `[#tag]` bracket-wrapped mono caps, in reading view and Live Preview.
- **Square geometry** throughout — no border radius; left-bar blockquotes, scan-line dividers, accent-tinted highlights.
- **Tier table, embeds, properties panel, mermaid** all themed.
- **`deepfield-components.css` snippet** — custom callout components (`attribution`, `hud`, `punchline`, `origin`, `bracket`, `transition`, `horizon`, `divider`, `entry`, `prose`) using native callout syntax, plus inline components (LED indicators, progress bars, code badges, scan lines, tier table).
- `EXAMPLE.md` live reference note.

### Notes
- Built on [Minimal](https://github.com/kepano/obsidian-minimal)'s HSL variable system; works standalone.
- Custom callout components require the `deepfield-components.css` snippet enabled.
- Mermaid is themed via `!important` overrides (Obsidian exposes no mermaid variables); labels are forced legible.

[1.0.0]: https://github.com/nbost130/deepfield/releases/tag/1.0.0
