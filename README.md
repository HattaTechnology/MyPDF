# MyPDF

**A free, lightweight PDF reader and editor for Windows.**
Version 1.10 — https://github.com/mus3na/MyPDF

Copyright (C) 2026 Hatta Technology. All rights reserved. For conditions of distribution and use, see License.pdf.

---

## Introduction

MyPDF is a professional yet lightweight PDF reader and editor built for Windows. It combines the essential features of a commercial PDF editor into a single clean interface — open, organize, edit, sign, watermark, redact, and print PDF documents without the bloat.

For full step-by-step instructions, see [Manual.pdf](Manual.pdf).

---

## Features

### View
- Open and read PDF files, including password-protected documents (3 password attempts).
- **Multiple documents in tabs** — each tab keeps its own undo history.
- Acrobat-style dark reading canvas with pages floating on soft shadows.
- **Zoom** 1–400 %, with **Fit Width** and **Fit Page** at the top of the zoom dropdown.
- **Hand tool** — drag to pan the page. Click the hand button, press `H`, or just hold **Space** while reading.
- Select text and copy it with `Ctrl+C` without switching to any edit mode.
- **Find** (`Ctrl+F`) highlights every hit and steps through them.

### Rotate
- **Whole document** — the two curved-arrow buttons on the toolbar rotate every page 90° left or right in a single undoable step.
- **Single page** — the rotate buttons inside the Edit panel turn only the page you are on.

### Organize Pages (`Ctrl+Shift+O`)
A thumbnail grid for restructuring documents:
- **Re-arrange** — drag and drop pages to a new position; a blue indicator marks the target slot.
- **Split** — right-click a page and choose *Split Here* to divide the document into two PDFs.
- **Insert / Merge** — right-click and choose *Insert Pages Before* to merge pages from another PDF.
- **Delete** — right-click and choose *Delete Page* to permanently remove a page.

### Edit PDF (`Ctrl+2`)
- **Add new text** — choose font, size, and colour, then click anywhere on the page.
- **Edit existing text** — hover to highlight an editable span, click to edit inline. Font matching maps serif → Times Roman, sans-serif → Helvetica, monospace → Courier.
- **Rotate page** — 90° increments, left or right (this page only).
- **Paste a picture** — snip anything with the Windows Snipping Tool and press `Ctrl+V`. It lands at its original size; drag to move it, drag the bottom-right handle to resize.

#### Annotation tools

All of these are real PDF annotations: they show up correctly in Acrobat, Edge or any other reader, they survive saving and reopening, and each one is a separate `Ctrl+Z` step. Only one tool is armed at a time — press `Esc` or right-click to put it away.

| Tool | How to use it |
|------|---------------|
| Tick (✓), Tick in Box (☑), Cross (✗) | Click on the page. Size comes from the **Size** box. |
| **Strike line** | Click to drop a line of the default length, or drag sideways to set the length exactly. The line always stays level. Click a line you already placed to select it, then drag the middle to move it or either end to change its length. |
| **Pen** | Draw freehand in the selected colour — circle a figure, jot a note, sign your name. Thickness is set by the **Pen width** box. |
| **Highlighter** | Swipe across text to highlight it in **yellow, green, blue or pink**. The highlight snaps neatly to whole words, and the text underneath stays selectable and searchable. |
| **Erase** | Click a pen stroke to delete it, or hold the button down and swipe across several. |
| **Move** | Drag any pen stroke to a new position. |

### Signature & Stamp / E-Sign (`Ctrl+E`)
- Load a scanned signature (Load Signature) or company chop (Load Chop) from PNG, JPG, or BMP.
- White / light backgrounds are removed automatically; transparent PNGs are kept as-is.
- Place, drag to reposition, and drag the corner handle to resize (aspect ratio preserved).

### Watermark (`Ctrl+W`)
Diagonal text watermark with configurable settings:

| Setting       | Description                                              | Default       |
|---------------|----------------------------------------------------------|---------------|
| Text          | Up to 50 characters                                      | CONFIDENTIAL  |
| Angle         | –180° to +180° (0° horizontal, 45° classic diagonal)     | 45°           |
| Font Size     | Point size of the watermark text                         | 30 pt         |
| Transparency  | Higher values produce a fainter mark                     | 80%           |

Apply to all pages or only the current page. *Remove Watermark* clears it.

### Redact (`Ctrl+D`)
Permanently obscures sensitive information by replacing the selected text with a solid black rectangle. The underlying text is **physically removed** from the PDF — it cannot be recovered by copy-paste or text extraction. Drag horizontally across the text to redact; the selection is locked to the line height.

> **Warning:** Once saved, redactions are permanent. Use *Save As* (`Ctrl+Shift+S`) to keep an unredacted copy.

### Print (`Ctrl+P`)
Print to any installed printer — choose printer, page range, and copies.

### Undo / Redo
Full session undo history covering text edits, page reordering, deletions, insertions, rotations, annotations, watermarks, redactions, and e-sign overlays.

| Action | Shortcut |
|--------|----------|
| Undo   | `Ctrl+Z` |
| Redo   | `Ctrl+Y` |

The history is cleared when you save and close, or open another file.

---

## Keyboard Shortcuts

| Action         | Shortcut         |
|----------------|------------------|
| Open           | `Ctrl+O`         |
| Save           | `Ctrl+S`         |
| Save As        | `Ctrl+Shift+S`   |
| Print          | `Ctrl+P`         |
| Find           | `Ctrl+F`         |
| Copy selected text | `Ctrl+C`     |
| Paste picture  | `Ctrl+V`         |
| Organize       | `Ctrl+Shift+O`   |
| Edit Text      | `Ctrl+T`         |
| E-Sign         | `Ctrl+E`         |
| Watermark      | `Ctrl+W`         |
| Redact         | `Ctrl+D`         |
| Comment        | `Ctrl+M`         |
| Undo / Redo    | `Ctrl+Z` / `Ctrl+Y` |
| Fit Page       | `Ctrl+0`         |
| Actual Size (100 %) | `Ctrl+1`    |
| Fit Width      | `Ctrl+2`         |
| Zoom in / out  | `Ctrl+=` / `Ctrl+-` |
| Hand tool (pan)| `H`, or hold **Space** |
| Cancel the current tool | `Esc` or right-click |

---

## System Requirements

| Component           | Minimum                          |
|---------------------|----------------------------------|
| Operating System    | Windows 10 (64-bit) or later     |
| Disk Space          | 200 MB free                      |
| Internet Connection | For downloading installer / updates |

---

## Installation

1. Download the latest installer from https://github.com/mus3na/MyPDF/releases.
2. Double-click `MyPDF_Installer_64.exe`.
3. When User Account Control prompts to allow software from an unknown publisher, click **Yes**.
4. Read and accept the license agreement, then click **Next**.
5. Choose the installation folder and click **Next**.
6. Select installation options and click **Next**.
7. Click **Install**. If a previous version is detected, the installer will prompt to uninstall it first — click **OK**.

---

## Updates

MyPDF does not include an automatic updater. To update:

1. Visit https://github.com/mus3na/MyPDF/Releases.
2. Download the new installer.
3. Run the installer.
4. Launch MyPDF and check the new version on the splash screen or under **Help > About**.

Updating does not affect existing PDF files. Application settings and recent file history are preserved.

---

## Saving Notes

- **Save** (`Ctrl+S`) overwrites the source file permanently.
- **Save As** (`Ctrl+Shift+S`) writes to a new file, keeping the original.
- All edits — organize changes, annotations, signatures, watermarks, and redactions — are held in memory until you save. Closing without saving discards them.

---

## Support & Feedback

MyPDF is free software distributed through GitHub.

- Repository: https://github.com/HattaTechnology/MyPDF
- Issues: https://github.com/HattaTechnology/MyPDF/issues
- Email: mus3na@msn.com

### Reporting Bugs
Please include:
- Your Windows version (Windows 10, 11, etc.).
- The steps that produce the bug (e.g., "Open file X, click Redact, drag across line 3").
- The exact error message from the status bar or any popup dialog.
- A screenshot of the problem if possible.
- A sample PDF if the bug is file-specific (or note if confidential).

---

© 2026 Hatta Technology. All Rights Reserved.
