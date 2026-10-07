# Changelog

All notable changes to Lerntafel are documented in this file. Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), versioning follows [SemVer](https://semver.org/) (beta versions as `0.MINOR.PATCH`).

## [0.9.6] - 2026-10-07

### Added
- **Page mode (A4):** the board as A4 sheets that behave like a document — the mouse wheel and touchpad scroll instead of zooming, content stays on the sheets, and new sheets appear only as you write. PDF pages sit directly on the sheets; export as a print-ready multi-page PDF (white paper, 300 dpi, lossless). The start page shows these boards as A4 sheets.
- **Split screen:** a PDF next to your note sheets, or next to a free board. Swap sides and drag the divider; each half has its own zoom and scrolling, and strokes stay within their half.
- **Help menu:** keyboard shortcut overview (F1), "Check for updates" and "About Lerntafel".
- **Update check:** Lerntafel checks this repository's releases at most once a day and shows a small notice with a download link when a newer version is available (see [PRIVACY.md](PRIVACY.md)).
- **Keyboard shortcuts** like in other drawing apps: Shift/Ctrl + corner keeps the aspect ratio, Alt scales from the center, Shift snaps rotation to 15° and locks moving to one axis; Ctrl+A/C/X/V/D, Esc, arrow keys (nudge the selection or pan the board), Ctrl+Plus/Minus, Shift+1 (fit all), Shift+2 (zoom to selection), F11 (full screen); tool keys P/E/V/T/H/L, colors 1–9, stroke width Ctrl+1–9; Ctrl+N/O/S/W/Tab for boards. Text copied from other programs can be pasted onto the board.
- Rotate a PDF by 90° from the bottom toolbar; rename a board from its tab menu.

### Changed
- Selections can be fully used with a finger: drag corners, rotate, delete and edit text.
- All pop-up messages now use the app's own style instead of the Windows message box.

### Fixed
- The live pen preview now matches the finished stroke exactly (including color zones, hold-to-straighten and shapes).
- Strokes drawn with pen pressure turned off no longer get thicker after undo, reloading or pasting.
- Cloze gaps on scanned worksheets with a halftone background are recognized.
- Resize cursors follow the selection's rotation; the selection frame follows a rotated PDF.
- A stroke that Windows never finishes after lifting the pen is now completed instead of leaving the board unresponsive.

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
