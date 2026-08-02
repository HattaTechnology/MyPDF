# MyPDF

**A free, lightweight PDF reader and editor for Windows.**
Version 1.03 — https://github.com/mus3na/MyPDF

Copyright (C) 2026 Ir. Ts. Musnazril Bin Mustaq Khan. All rights reserved. Portions Copyright (C) 2026 mus3na. All rights reserved. For conditions of distribution and use, see License.pdf.

---

## Introduction

MyPDF is a professional yet lightweight PDF reader and editor built for Windows. It combines the essential features of a commercial PDF editor into a single clean interface — open, organize, edit, sign, watermark, redact, and print PDF documents without the bloat.

For full step-by-step instructions, see [Manual.pdf](Manual.pdf).

---

## Features

### View
- Open and read PDF files, including password-protected documents (3 password attempts).
- Standard reader view with title bar showing the file name and a status bar showing the page count.

### Organize Pages (`Ctrl+Shift+O`)
A thumbnail grid for restructuring documents:
- **Re-arrange** — drag and drop pages to a new position; a blue indicator marks the target slot.
- **Split** — right-click a page and choose *Split Here* to divide the document into two PDFs.
- **Insert / Merge** — right-click and choose *Insert Pages Before* to merge pages from another PDF.
- **Delete** — right-click and choose *Delete Page* to permanently remove a page.

### Edit PDF (`Ctrl+2`)
- **Add new text** — choose font, size, and colour, then click anywhere on the page.
- **Edit existing text** — hover to highlight an editable span, click to edit inline. Font matching maps serif → Times Roman, sans-serif → Helvetica, monospace → Courier.
- **Rotate page** — 90° increments, left or right.
- **Annotation** — place vector symbols permanently onto the page:
  - Tick (✓)
  - Tick in Box (☑)
  - Cross (✗)
- **Ink** — use ink to sketch anything above pdf.
- **Highlighter** — highlight any text.

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

### Comment
User can place comment and edit existing comment.

### Search
User can now search the whole PDF.

---

## Keyboard Shortcuts

| Action         | Shortcut         |
|----------------|------------------|
| Open           | `Ctrl+O`         |
| Save           | `Ctrl+S`         |
| Save As        | `Ctrl+Shift+S`   |
| Print          | `Ctrl+P`         |
| Organize       | `Ctrl+Shift+O`   |
| Edit mode      | `Ctrl+2`         |
| E-Sign         | `Ctrl+E`         |
| Watermark      | `Ctrl+W`         |
| Redact         | `Ctrl+D`         |
| Undo / Redo    | `Ctrl+Z` / `Ctrl+Y` |

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

- Repository: https://github.com/mus3na/MyPDF
- Issues: https://github.com/mus3na/MyPDF/issues
- Email: mus3na@msn.com

### Reporting Bugs
Please include:
- Your Windows version (Windows 10, 11, etc.).
- The steps that produce the bug (e.g., "Open file X, click Redact, drag across line 3").
- The exact error message from the status bar or any popup dialog.
- A screenshot of the problem if possible.
- A sample PDF if the bug is file-specific (or note if confidential).

---

© 2026 Ir. Ts. Musnazril Bin Mustaq Khan. All Rights Reserved.
