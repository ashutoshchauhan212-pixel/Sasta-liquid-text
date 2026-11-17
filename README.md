# pranav — PDF + Freeform-style workspace (V6)

This version keeps Apple Pencil input as raw freehand ink strokes. There is no handwriting-to-text conversion.

## Right-side canvas
- Freehand pen strokes with pressure-sensitive width when the browser reports Apple Pencil pressure.
- Highlighter and broad-stroke eraser.
- Ink colour and width controls.
- Undo and redo for ink.
- Freehand ink is saved locally in IndexedDB and included in workspace JSON export.
- Double-click empty canvas to add a separate typed note object.
- Drag and resize notes, excerpts and clipped image objects.
- PDF area clipping creates a movable image object on the workspace.

## Run
Open `index.html` in Safari or Chrome. PDF.js is loaded from a CDN, so initial PDF rendering needs internet. For PWA install/service worker, serve over HTTPS or localhost.

## Platform limitations
This is a browser implementation, not Apple's native Freeform engine. Safari exposes Apple Pencil as Pointer Events on supported iPadOS versions, but advanced native Freeform capabilities such as full palm rejection tuning, hover, tilt/azimuth fidelity, native object connectors, collaboration and system-level PencilKit integration are not guaranteed. No OCR or handwriting conversion is performed on ink strokes.
