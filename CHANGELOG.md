# Changelog

All notable changes to this theme are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/),
and this theme adheres to [Semantic Versioning](https://semver.org/).

## [1.0.3] - 2026-11-23

### Added
- **Repository hero banners.** Added light and dark landscape banners (`images/banner-light.webp` and `images/banner-dark.webp`, strictly aligned at 2688 × 864) embedded at the top of `README.md` with automatic light/dark mode adaptation.

### Changed
- **Font settings & inheritance.** Removed hardcoded `--font-text`, `--font-ui`, and `--font-monospace` overrides from `.theme-light` and `.theme-dark`. Reading view (`.markdown-preview-view`) now adheres to `var(--font-text)` (matching Live Preview), and interface components (`.workspace`, `.workspace-sidedock`, `.titlebar`, `.status-bar`, `.metadata-container`) adhere to `var(--font-ui)`. Custom font overrides in Obsidian Appearance settings now take effect seamlessly across all views while preserving the default LXGW WenKai / JetBrains Mono fallback.
- **Tasks query panel border.** The ` ```tasks ` block rendered by the Tasks
  plugin (`.block-language-tasks`) now gets an outer border in the theme's
  standard modifier color, so the query result reads as a self-contained panel.

## [1.0.2] - 2026-09-04

### Changed
- **Toggle switches now read as neutral gray when off.** The settings-pane switch
  (`.checkbox-container`) previously inherited `--background-modifier-border`,
  which this theme tints green — so a switched-off control still looked green.
  The off state is now a neutral gray and forest green is reserved for the on
  state, keeping the accent meaningful.
- **Task checkboxes** (`.task-list-item-checkbox`) use a neutral gray outline when
  unchecked, darkening on hover to signal they are clickable. The checked state
  keeps its forest-green fill.
- **Dark-mode check-mark contrast**: the tick on a checked task box is now
  ink-dark (`#1a201c`) rather than near-white, because the dark-mode checked
  ground is a bright forest green (`#7dba8b`). Light mode is unchanged.

### Documentation
- Merged `README.zh.md` into `README.md` as a single bilingual document
  (English first, Chinese after) and removed the separate Chinese file.
- Removed the *Compatibility*, *Project Structure*, and *Publishing* sections and
  dropped the "(pending submission)" wording from the install instructions.

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
