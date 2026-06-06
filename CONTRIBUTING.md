# Contributing to Deepfield

Thanks for your interest in improving Deepfield.

## Reporting issues

Use the issue templates — **Bug report** for something rendering wrong, **Feature request** for new palettes, components, or element coverage. Screenshots help enormously; include your Obsidian version, whether you're in light or dark mode, and which palette is active.

## Making changes

The theme is hand-written CSS — no build step.

- **`theme.css`** — the theme itself. Targets `body.theme-dark` for the dark base and `body.theme-light` for light; component rules are theme-agnostic (`body .selector`) and pull colors from CSS variables so they adapt to both modes and all 20 palettes.
- **`deepfield-components.css`** — the optional snippet adding custom callout + inline components. Must stay standalone-safe (use `var(--x, fallback)` form) so it works on any theme.
- **`EXAMPLE.md`** — the live reference note. If you add or change an element, update this so the change is verifiable in a real vault.

### Conventions

- **No hardcoded accent colors.** Use `rgba(var(--interactive-accent-rgb), α)` so every palette recolors correctly — never a literal `rgba(29,111,255,…)`.
- **Square geometry** — no `border-radius` on new elements.
- **Palette accents are theme-agnostic; backgrounds and text belong to the mode blocks.** Don't add background/text values to palette blocks.
- Verify changes in **both light and dark**, and on at least one non-Electric palette (e.g. Mars), before opening a PR.

## Releasing (maintainers)

1. Bump `version` in `manifest.json` and add the matching `versions.json` entry.
2. Add a `CHANGELOG.md` entry.
3. Tag the commit with the exact version (`git tag 1.1.0 && git push origin 1.1.0`). The release workflow validates the tag matches the manifest and publishes `theme.css` + `manifest.json`.

## License

By contributing you agree your work is licensed under the [MIT License](LICENSE).
