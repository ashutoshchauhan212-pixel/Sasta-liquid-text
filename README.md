# pranav — PDF + Freeform workspace V7

The right side is a freeform canvas, not a required note-card editor.

- Apple Pencil (pen pointer) draws directly onto the canvas as persistent ink strokes. No OCR, transcription or handwriting-to-text conversion.
- Finger touch is reserved for scrolling/panning the canvas. This avoids accidental finger marks while writing with Pencil.
- Cards and image/text objects sit above the ink layer and remain selectable/draggable.
- Pencil, highlighter, eraser, undo/redo, colour and width controls.
- Add independent typed text objects with `A Text`.
- Crop rectangular image regions from the PDF and move them on the canvas.
- Typed notes, excerpts, clipped images and ink persist locally; export includes ink.

## Deployment
Replace the existing GitHub Pages files with `index.html`, `manifest.json`, and `sw.js`. Commit and wait for Pages deployment. Then on iPad Safari, reload the site. If the old interface persists, close the old tab and reopen the Pages URL; optionally clear the site's cached website data.

## Important platform boundary
This is a web implementation, not Apple's native Freeform or PencilKit. It uses browser Pointer Events and pressure values where Safari supplies them. Native Freeform's exact palm rejection, tilt/azimuth, hover, collaboration and system integration cannot be guaranteed in a web app.
