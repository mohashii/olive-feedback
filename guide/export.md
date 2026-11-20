# Export

Olive exports a note as it looks on screen, as a single HTML file or as a PDF. Exporting never changes the `.md` file.

## HTML

The HTML file is self-contained. Images are embedded, the math fonts and styles travel with it, and Mermaid diagrams are baked in as pictures, so it opens with no network connection and the math still renders. Images referenced by an `https://` URL are the one exception: Olive does not fetch them, and marks where they were instead. Front matter is never included.

At the end of the page, a **Save Markdown** button lets the reader download the note's Markdown source, embedded in the file itself so it works offline. You can instead offer a `.zip` with the images as well, or leave the button out.

## In the Mac app

- **A note** — **File → Export as HTML…** or **File → Export as PDF…**. The PDF is made by macOS itself, so no browser is needed.
- **A whole folder** — **Export as HTML…** in a folder's right-click menu, or in the menu on the folder name at the bottom of the sidebar for everything. You choose which notes to include, and Olive writes one HTML file with a sidebar for moving between them.
- **The Save Markdown button** is set in **Settings → What to add to the end of an exported HTML file**: nothing, a **Save Markdown** button (the default), or a **Save Markdown and images** button that downloads a `.zip`.

## In VS Code

Run **Olive: Export as HTML** or **Olive: Export as PDF** from the Command Palette while an Olive editor is active.

- **The Save Markdown button** is set by `olive.export.includeSource`: `markdown` (the default), `archive` for a `.zip` with the images, or `none`.
- **PDF** is rendered by a Chromium-based browser. Olive looks for one you already have — Chrome, Chromium, Edge, Brave, Arc, Vivaldi or Opera, including their Beta, Dev and Canary channels — and uses it without asking. If it finds none, it offers once to download a print-only engine of about 100 MB; you can decline and use **Export as HTML** with your browser's own print-to-PDF instead. To point Olive at a browser it did not find, set `olive.pdf.executablePath` to the executable; on macOS that is the file inside the app bundle, such as `/Applications/Arc.app/Contents/MacOS/Arc`, not the `.app`. **Olive: Update PDF engine** downloads the engine again and removes the old one.

---

Back to the [contents](README.md).
