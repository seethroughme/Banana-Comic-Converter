# Banana Comic Converter

Turn comic and manga files (CBZ, ZIP or PDF) into pages that fill an e-ink screen, or into a long scrolling PDF for your phone. It can find each panel and fit it to the screen, automatically choose halves or thirds for every page, or simply cut every page into overlapping parts. Output as XTCH or XTC (Xteink devices), EPUB, CBZ or webtoon PDF, in black and white or colour.

**Everything runs in your browser. Nothing is uploaded and nothing is installed. No AI is used anywhere in the conversion: panels are found with plain image analysis (whitespace and border detection) that runs on your device, with no AI model and no online service.**

**Live site: https://seethroughme.github.io/Banana-Comic-Converter/**

Use it only with files you own or have the right to convert for personal use.

If it saves you time: [Buy me a coffee](https://ko-fi.com/curseofthebanana)

---

## Quick start

The page walks you through four steps.

1. **Add your files.** Open the [live site](https://seethroughme.github.io/Banana-Comic-Converter/) (or open `index.html` locally in any modern browser). Drop CBZ, ZIP or PDF files on the box, or click it to browse. Folders work too.
2. **Choose your device.** Pick a quick setup (Xteink X3 or X4, Kindle, Kobo, Boox, phone and more) or enter a custom screen size. Pick the reading direction (right-to-left for manga). Your last device is remembered.
3. **Choose the output.** Tick the screen shapes (Portrait, Landscape, Mixed) and file types (XTCH, XTC, EPUB, CBZ, webtoon PDF). One file is made for every combination.
4. **Choose how pages are cut.** Pick **Smart panels**, **Smart halves and thirds** or **Simple page split** (see below).

Tick "I own these files", press **Convert**, then download. For batches, use "Download all as one ZIP". You can cancel at any time. Less common settings are tucked into **More options**.

The small **i** next to each section explains it. **How to use**, **Tips and fixes** and **What's new** at the top open the in-app guides.

## Three ways to cut pages

**Smart panels** detects panels, orders them for your reading direction, packs small panels together and enlarges long ones. A page-by-page editor lets you fix mistakes.

**Smart halves and thirds** skips panel boxes and chooses, for every page, whether to show it whole, in halves or in thirds. Cuts are placed in blank gaps so speech bubbles stay whole, and parts are sized to fill the screen width for the orientation you chose (portrait, landscape or mixed). You can preview every page, and set Auto, No zoom, Halves or Thirds page by page.

**Simple page split** cuts every page into 2 (halves) or 3 (thirds) overlapping parts in reading order (overlap 8%, 15% or 25%), optionally after showing the whole page. Landscape screens get top-to-bottom bands; portrait screens show pages whole (wide spreads are cut left and right). Good for a quick conversion.

## Features

- **Input:** CBZ, ZIP (png, jpg, webp, gif, bmp) and PDF. Batch conversion, natural page sorting, cover first, credit pages last. Chapters from file or folder names, or PDF bookmarks. Title and volume can be read from the file name.
- **Batch edits:** when you add several files, each gets its own title and volume field, so a whole series can be named properly in one run. Fields you fill in elsewhere (author, series, publisher and so on) are applied to every file, and any you leave blank keep each file's own value. Panel edits, hidden pages and zoom choices are also kept separately for every file in the batch.
- **Metadata:** title, author, series, volume, publisher, year, language and description are read from the file where it has them (ComicInfo.xml, PDF properties) and filled in automatically, otherwise the title comes from the file name. You can edit any field before converting. Metadata is stored in EPUB, CBZ (ComicInfo.xml) and PDF; XTCH and XTC keep title, author, publisher and language.
- **Output formats:** XTCH (4-level grey), XTC (pure black and white, with an adjustable cutoff or an Auto button), EPUB, CBZ and webtoon PDF. Big books can be split into parts to fit low-memory devices.
- **Webtoon PDF:** panels are cut out and stacked in reading order into tall strips, so you can scroll a chapter on a phone. Pick the width, and choose panels or whole pages.
- **Colour or black and white:** devices with black and white screens (Xteink, Kobo Libra 2, Clara BW and so on) default to black and white. For colour devices and phones you can keep colour in EPUB, CBZ and PDF. XTCH and XTC are always grey.
- **Screens:** Portrait, Landscape, or **Mixed** (wide panels on landscape screens, tall panels on portrait screens, in one file). Many device presets, a custom size, and a direction test so you can check left-to-right against right-to-left on a sample page.
- **Size estimate:** an estimate of file size and screen count before you convert, with warnings for files that may be too big for a device.
- **Pages manager:** drag pages to reorder, hide ads and credits, choose the cover, and scan for blank pages. Choose pages to show whole instead of cutting them into panels.
- **Panel detection:** whitespace gutters with a fallback for busy pages, automatic detection of black gutters, reading order that handles tall panels beside stacked ones.
- **Zoom and splitting:** long panels are shown whole, then as two enlarged halves. Optional dense page zoom shows crowded screens whole, then as zoomed tiles. Cuts snap to blank gaps so speech bubbles stay whole where possible.
- **Packing:** small panels share a screen (max 1, 2 or 3) when they stay large enough.
- **Panel editor:** move, resize, draw, delete and reorder boxes; merge boxes; split a box by drawing a line; box shape lock to your screen's proportions; undo; a preview of the screens each box becomes. All controls sit in one side column next to the page, with a progress bar for flagged, reviewed and remaining pages.
- **Review grids:** see every page's boxes, or every page's zoom choice, in one grid, and jump straight to any page.
- **Zoom per box and per page:** pick Auto, Off, overlapping Halves or overlapping Thirds for a single box, or for a whole page in the smart halves and thirds mode.
- **Spoiler blur:** a toggle and a slider blur artwork and text while keeping panel outlines visible, so you can edit and review without spoiling the story. Works in the editor, the review grids, the cut preview and the Pages thumbnails.
- **Pages to check:** flags pages with several panels in one box, very big boxes or overlapping boxes (tall and busy boxes optional), or filters pages by panel count. Step through flagged pages only.
- **Keyboard shortcuts:** arrows change page, up/down or 1-9 pick a box, H / T / O / A set zoom, **G** re-detects with black gutters (R goes back to normal), B toggles the blur, plus D, W, R, S, F, M, C, [ ], Delete and Ctrl+Z. The keys are shown on the buttons.
- **Image quality:** sharpen, e-ink contrast, darker midtones, screentone moire reduction, auto-levels, JPEG quality, and XTCH dither styles, with a before and after quality preview.
- **Cover:** kept whole on a portrait page in landscape and mixed output.
- **Saved presets:** store all settings under a name (kept in your browser), and export or import presets as a file to move them between browsers.
- **Progress saving:** your panel edits, hidden pages, page order and zoom choices are saved in your browser as you work, and come back when you open the same file again, even after converting. This needs your browser to allow site storage for the page (see below).
- **Faster conversion:** on computers with several cores, screens are drawn and encoded in parallel, and panel detection is remembered so the same page is not analysed twice. A switch in More options turns this off if a very large book runs out of memory.

## File types

| Type | Notes |
|------|-------|
| XTCH | 4-level gray container for Xteink devices. Landscape pages are stored sideways, so turn the device to read them. Options: rotation, dither style, experimental cover thumbnail. |
| XTC | Pure black and white (1-bit) container for Xteink devices, with an adjustable black and white cutoff. |
| EPUB | Fixed layout with a chapter table of contents and full metadata. Colour or black and white. |
| CBZ | Plain image pages plus a ComicInfo.xml. Colour or black and white. |
| PDF (webtoon) | Panels or whole pages stacked into tall strips for scrolling on a phone. Colour or black and white. |

The XTCH and XTC output follows a community-written format description and has not been tested on every device. The cover thumbnail option is experimental. EPUB readers may not rotate automatically for mixed output.

## Known limits and what to expect

This is a hobby tool, not a finished product. It uses ordinary image analysis, with no AI, so it follows rules rather than understanding the page. It works best on pages with clear white or black gaps between panels.

**Panel detection**
- Most pages come out right, but some will need a fix in the editor. In a test on a real 204-page manga volume, roughly 1 page in 4 was flagged for a manual look. Not every flagged page was actually wrong.
- Panels with no borders, artwork that bleeds into the next panel, or panels that sit on top of each other can get a box that is slightly too big, too small or overlapping. Inset panels over a full-page drawing and full-bleed or slanted layouts are the usual case.
- Several panels can be merged into one box, or one panel split in two, especially on busy or very dark pages.
- Reading order is a best guess. Unusual layouts can come out in the wrong order. The editor has **Sort order** and **Earlier / Later** to fix this.
- Splash pages, double-page spreads and pages with large sound effects may be treated as one big panel, or cut in odd places.
- Speech bubbles and text can be cut when a long panel or a zoom is split. Cuts move to blank gaps where there are any, otherwise they overlap. A larger overlap helps. Smart halves and thirds can still occasionally leave a bubble at the edge of a part, so use the preview on important pages.
- The page-flagging checks are tuned on a small set of pages. Treat flags as hints, not a guarantee, and page through anything important.

**Output**
- XTCH and XTC follow a community description of the format. They have not been tested on every Xteink device or firmware, and the exact memory limit of each device is not known. Try a short file first, and use "split into parts" if a device runs out of memory.
- Mixed-orientation EPUB asks the reader to rotate per page, but not every reader does. If yours doesn't, use portrait or landscape output instead.
- Landscape XTCH pages are stored sideways, so you turn the device to read them.
- Greyscale and dithering change how fine detail and screentone look on e-ink. Try the dither and moire settings if a page looks muddy. Moire reduction is skipped for colour output.
- Colour output has not been tested on every colour e-ink reader. Colour pages use about four times as much memory while converting.

**Size and speed**
- Everything is converted in your browser's memory, so big books are slow and use a lot of RAM. Speed depends on your computer: parallel processing helps most on computers with several cores. On a small 2-core test machine a 204-page volume converted to two outputs in about 50 seconds. Phones and low-memory devices may stall on very large files, so convert in chunks or one output at a time.
- Output files are large because pages are stored as images.

**Saved progress**
- Edits are saved in your browser's site storage (IndexedDB), on that device only. A file is recognised by its name and size. Saving does not work if your browser blocks site storage for the page or you are in a private window, and clearing site data removes saved edits. They are not moved between devices or browsers.

**Other**
- Tested mainly in Chromium (Chrome, Edge). Safari, Firefox and mobile browsers have had little testing, so layout or memory limits may differ.
- Scanned PDFs are converted as page images. There is no text extraction or OCR.
- Use only files you own or may convert for personal use.

If something fails, open an issue and include a sample page (or a description of the layout), the settings you used, and the device or reader you tried it on.

## Your data

- Files are read and converted locally in your browser. Nothing is uploaded or shared.
- No AI or machine learning is used during conversion. Detection is ordinary image analysis, so results are repeatable and you can correct any page in the editor.
- Presets, your last device, the spoiler blur setting, which sections are open and your saved edits are kept in your browser's storage on that device only. Clearing site data removes them. The **Forget saved edits** button deletes saved edits for the selected files.
- The only outside link is the Ko-fi button.

## Credits and licences

- PDF reading uses [PDF.js](https://mozilla.github.io/pdf.js/) by Mozilla (Apache License 2.0), bundled in the page.
- Not affiliated with any device maker or publisher. Product and device names belong to their respective owners.
