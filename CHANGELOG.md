# Changelog

All notable changes to this theme are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/),
and this theme adheres to [Semantic Versioning](https://semver.org/).

## [1.0.1] - 2026-07-31

### Changed
- Source-mode (plain text editing) blockquotes now render as a continuous panel
  matching the reading-view style, via `:has()` line washing. (Requires Obsidian
  1.1.9+ / Electron 21, which supports `:has()`. Live Preview blockquotes were
  already matched.)

## [1.0.0] - 2026-07-17

First release of **林栖 (ForestRest)** — a serene "dwell-in-the-woods" Obsidian
theme, ported from the Typora theme *lightmind* (clear / light mind → dwelling
in the woods).

### Added
- **Warm beige rice-paper surface** (`#f4f1e8` / `#faf7ef`) for low-fatigue long reading.
- **Forest-green accents** (林绿 `#4a7c59` / 深林 `#234a31` / 新苔 `#8fb39b`), used sparingly as foliage peeking through the paper.
- **Ink code blocks** — the *"ink block on rice paper"* (宣纸上的墨块) motif. In **dark** mode the block is ink-black (`#232220`); in **light** mode the same block uses a soft forest-green ground (`#d6e7d6`) so code stays gentle on the pale page.
- **Body in LXGW WenKai (霞鹜文楷)**, **code in JetBrains Mono** — warmth of a soft brush against the precision of hard ink.
- **Forest-spectrum syntax highlighting**: 苔紫 / 秋金 / 新生苔 / 赭石 / 溪青 / 暖陶, tuned per mode (a luminous spectrum on the dark ink ground, deeper forest greens on the light ground).
- **Full theming** for Callouts, tables, blockquotes, tags, math, and footnotes.
- **Light-primary** design plus a derived "night forest" (夜林) dark mode (`#161b18`), both from one forest palette.
- **Pure local font fallback chain** — no external network dependencies.
- `versions.json` for Obsidian version → theme version compatibility mapping.
- Concept preview and light / dark interface screenshots under `images/`.
