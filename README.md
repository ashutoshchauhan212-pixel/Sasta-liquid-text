# pranav — PDF + writing canvas

Upload these files to the root of your existing GitHub Pages repository, replacing `index.html` and updating `manifest.json` and `sw.js`.

## What this build does
- Two-pane layout: PDF on the left, freeform writing canvas on the right.
- PDF rendering with PDF.js; selectable text layer over rendered pages.
- Select text in the PDF and tap **Add selected text** to create a movable excerpt card on the canvas.
- Add freeform note cards; type into them and drag their headers to move them.
- Local IndexedDB storage, backup and restore.
- Reuses the existing `pranav-legal-workspace` database and `items` store so earlier imported PDFs should remain available.

## Important
- PDF.js is loaded from a CDN. Internet is needed to load the PDF engine; full offline PDF operation is not yet implemented.
- On iPad, select text by touch and use **Add selected text**. Dragging excerpt cards by their header moves them on the canvas.
- This prototype supports text excerpts, not yet image-region clipping, Apple Pencil ink, card resizing, or infinite-canvas zoom/pan. Those are next milestones.
- Keep backups of important documents.
