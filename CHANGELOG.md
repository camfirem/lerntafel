# Changelog

All notable changes to Lerntafel are documented in this file. Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), versioning follows [SemVer](https://semver.org/) (beta versions as `0.MINOR.PATCH`).

## [0.9.5] - 2026-09-30

### Added
- Markdown tables in AI chat replies now render as real tables (bold header, thin borders, formulas and bold text in cells), scroll sideways when wide, and text inside a cell can be selected and copied.
- Pen and finger now scroll and select naturally throughout the chat, including a swipe-with-momentum feel.

### Changed
- Rotated snapped shapes (rectangle, triangle, etc.) by dragging further while the pen is still down; near-horizontal/vertical rotation snaps straight.

### Fixed
- PDF worksheets: cloze gaps in running text and right after a word are now recognized as answer fields; two-column worksheets no longer miss an answer line or mislabel it from the neighboring column; AI answers without a detected field stay on the PDF page instead of drifting next to it.
- PDF: ink stays black across light/dark theme switches instead of turning white and disappearing on the page.
- Single-page vs. "whole PDF" view: notes, strokes and shapes now move to their correct page when switching views instead of overlapping; selection and eraser only affect the visible page.
- AI corrections on the board keep their original color and starting position instead of resetting to black or shifting.
- Arrow detection no longer mistakes a loop or a long curve for an arrowhead; drawing can resume after a shape briefly snaps mid-stroke without leaving a stray line.
- Toolbars no longer get stuck unresponsive after a finger swipe across the board.

## [0.9.4] - 2026-09-27

First public beta release.

### Added
- English user interface, selectable during setup or later in Settings → Language.
- Real LaTeX-style math typesetting on the board (tall brackets, stacked limits, sums/integrals, matrices/cases) and in the AI chat.
- Automatic column layout for multiple tasks written to the board at once.

### Fixed
- Free board text layout no longer overlaps PDF pages.
- Inline task headings now get their own line instead of running into the formula.

### Known issues
- Installer is not code-signed yet; Windows SmartScreen will show a warning on first run (see [README](README.md#download)).

<!--
## [0.9.6] - YYYY-MM-DD

### Added
### Changed
### Fixed
### Known issues
-->
