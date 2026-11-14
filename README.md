# BarCraft

**A barcode maker that runs in your browser.**

BarCraft creates the full supported set of bwip-js symbologies: linear
barcodes, GS1 codes, 2D / QR codes, postal barcodes and HIBC variants.
Barcodes are drawn as exact vector bars so they never blur, then exported at
203 / 300 / 600 DPI as PNG, JPG or SVG.

## Getting started

1. Double-click `index.html`. It opens in Chrome or Edge.
2. Pick a barcode type on the left, or use the **Insert** ribbon tab.
3. Change the value, size and (for linear codes) the text font in the right
   panel, then **Output > PNG / JPG / SVG**.

Everything runs offline from this folder.

BarCraft autosaves the current canvas to your browser while you work. When
you open `index.html` again, it restores that last autosaved session
automatically. Use **File > Reopen last used…** or the left-panel
**Reopen last used…** button if you started a clean sheet and want the
previous work back; use **File > New** for a clean sheet.

The **Insert** tab opens a searchable barcode dialog grouped by family, and
the left type panel has its own search box. The same tab also has **Shapes**
(rectangle, square, circle and hexagon), **Text**, and **Artwork** (SVG, PNG,
JPG, WebP, GIF, BMP files or ClipArtCraft image links). Ribbon sections use
dropdown menus and dialogs to keep the workspace clean on any screen size.

Standard-purpose barcodes (postal, retail, GS1, ISBN/ISSN/ISMN, pharmaceutical,
HIBC, shipping and 2D content formats) show their required data format in the
insert dialog, type list, and properties panel.

The left barcode type panel is grouped and collapsible. The right panel has
**Details** and **Layers** tabs: Details shows the selected object, document,
barcode or shape controls; Layers shows the full stacking order with reorder
buttons. The bottom status bar shows the document size, live element/type
counts, and zoom controls with a type-in percentage and one-click fit.

## Mobile, tablet and touch

The same single-file app adapts to phones, slates, laptops and clamshells.
On narrow screens the type and properties panels become touch drawers, the
ribbon becomes a compact horizontally scrollable toolbar, and dialogs stay
inside the viewport with their own scrolling. Touch targets are enlarged for
coarse pointers, and the canvas automatically fits the available space.

## What is included

- **Linear**: Code 128, GS1-128, Code 39 / 93 (with and without full ASCII),
  Code 11, Codabar, Code 2/5, Interleaved 2/5, IATA 2/5, Matrix 2/5, ITF-14,
  EAN-13 / 8 / 2 / 5, ISBN, ISMN, ISSN, UPC-A / E, MSI, Pharmacode,
  Pharmacode2, Plessey, Telepen / Telepen Numeric, PosiCode, BC412, Code 16K,
  Code 49, Channel Code, DAFT, PZN, Leitcode, Identcode and Flattermarken.
- **2D & QR**: QR Code, Micro QR, PDF417, Micro PDF417, PDF417 Compact,
  Data Matrix (square, rectangular and rectangular extension), Aztec, Aztec
  Compact, Aztec Rune, MaxiCode, Han Xin, DotCode, Code One, UltraCode,
  Codablock F, GS1 QR and GS1 Data Matrix.
- **Postal**: Postnet, PLANET, OneCode, Royal Mail, KIX and Japan Post.
- **HIBC**: Code 128, Code 39, Codablock F, Aztec, Data Matrix, Micro PDF417,
  QR Code and PDF417 variants.
- **Drawing**: rectangle, square, circle and hexagon shapes with solid fill,
  outline, outline width, rounded corners for rectangles/squares, and
  multi-stop linear or radial gradients with per-stop transparency.
- **Text**: add editable text boxes in any local font, with size, colour,
  bold/italic/underline and left / center / right / justified alignment.
- **Dingbats**: add symbol glyphs using the bundled `Yarndings`,
  `Noto Sans Symbols 2`, and `Noto Emoji` fonts from the local archive.
- **Layout**: align selected objects left / center / right / top / middle /
  bottom, distribute them horizontally or vertically, and manage the full
  stacking order with a layer tree or right-click context menu.
- **Effects & editing**: apply drop shadows to any selected object, use the
  **Edit** ribbon for text style / alignment / colour and object effects, and
  filter or collapse the right properties panel with its search box and
  collapsible sections.
- **Barcode text**: for linear barcodes, keep the human-readable text below or
  beside the barcode, choose any local font, set text size and text colour,
  and toggle it on/off independently of the bars.
- **Artwork**: import SVG, PNG, JPG, WebP, GIF and BMP files, or use an image
  URL from ClipArtCraft / another source.

## Data

- Type any value directly into the right panel.
- For 2D codes, use the **Standard format** picker for web addresses, email,
  phone, text messages, Wi-Fi, contact cards (vCard) and map locations. Postal,
  EAN/UPC, ISBN, GS1 and HIBC codes show the format they need right in the
  panel.
- Use the **Arrange** tab or the right-hand **Object** panel to rotate by any
  angle (including 90, 160, 240 and 320 degrees), flip horizontally or
  vertically, invert or reset colours, and send objects backward / forward /
  to the back / to the front.
- Right-click an object for its most-used actions, or right-click empty canvas
  to insert objects; the **Layers…** dialog shows the complete stacking order.
- Add full-page colour backgrounds, black or white canvas backgrounds, and
  recolour barcode bars, shape fills, and shape outlines from the panels.
- Use **Data > Numbering / series** to make a run of sequential barcodes.
- Use **Data > Import CSV** to bring in a CSV address list, choose one column
  or combine several columns (with a separator) and generate one barcode per
  row. Header rows and quoted fields are handled automatically.

## Document sizes and output

- **Label stock** picker with common Dymo LabelWriter, Dymo D1, Brother DK,
  Brother TZe, Zebra / thermal, Avery US Letter and Avery A4 sizes, plus
  Letter/A4 page sizes.
- **Custom sizes** in millimetres or inches, with a one-click **Turn 90°**.
- **Print** at the label's real size, or export PNG / JPG / SVG at 203, 300
  or 600 DPI.

## Fonts

Linear barcodes with human-readable text can use every font in the local
`fonts/` archive through the **Text font** picker.

## Keyboard shortcuts

- `Ctrl+Z` / `Ctrl+Y` — undo / redo
- `Ctrl+C` / `Ctrl+X` / `Ctrl+V` — copy / cut / paste selected barcode(s)
- `Ctrl+D` — duplicate selected barcode(s)
- `Ctrl+A` — select all barcodes on the page
- `Delete` / `Backspace` — delete selected barcode(s)
- `Ctrl+Shift+V` — paste multiple values from the clipboard (one per line)
- Arrow keys move the selected barcode(s); `Shift` + arrows move in larger steps
- `[` / `]` send selected objects backward / forward, `{` / `}` send them to
  the back / front
- `H` / `V` flip selected objects horizontally / vertically
- `I` invert selected objects; `R` open the rotate dialog
- `Ctrl+[` / `Ctrl+]` send selected objects one layer backward / forward;
  `Ctrl+{` / `Ctrl+}` send them to the back / front
- `+` / `-` zoom in / out, `0` fit to window, `Esc` clear selection

## How it is built

- Source: `barcraft.src.html` (HTML, CSS and JavaScript in one file).
- `python build.py` writes:
  - `index.html` (offline, libraries from `lib/`)
  - `dist/artifact.html` (libraries from cdnjs)

Libraries: Fabric.js 5.3.1, JsBarcode 3.11.6, qrcode-generator 1.4.4,
bwip-js 4.10.2 (all MIT). Fonts come from the local `fonts/` archive.
