# pranav — PDF thinking workspace

An iPad-first, dark-mode, browser-based PDF + freeform notes workspace.

## Run
- Open `index.html` in a modern browser (PDF.js is loaded from a CDN, so the first run needs internet).
- For PWA installation/offline shell caching, serve this folder over HTTPS or localhost.
- On iPad Safari: open the hosted page, Share → Add to Home Screen.

## Included
- Two-pane PDF and freeform workspace, adjustable split.
- PDF page navigation and zoom.
- Selectable PDF text layer; send selected text into movable excerpt cards.
- Free-writing cards, edit-in-place, drag, resize, duplicate and delete.
- IndexedDB local workspace persistence.
- JSON workspace export.
- Basic PWA manifest and service worker.

## Important current limitations
This is a functional foundation, not a claim of feature-for-feature LiquidText parity. In this build, PDF text extraction is supported; image-region clipping, Apple Pencil handwriting/ink, multi-document linking, cross-page excerpts, full-text search, and PDF annotation/highlight export are not implemented yet. PDF rendering and text selection depend on the PDF.js CDN being reachable.
