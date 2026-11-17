# pranav — first working prototype

A personal, dark-mode, local-first legal research PWA prototype for iPad.

## Included in this first version
- Import PDFs into browser-local IndexedDB
- List and reopen imported PDFs
- Extract selectable text from the currently displayed page
- Save extracted passages as research cards
- Add notes to each passage
- Export a JSON backup containing PDFs and research cards
- Basic app shell caching for repeat visits

## Important prototype limitations
- PDF pages are currently presented as selectable extracted text, not as full-fidelity rendered page images.
- Search currently checks only the displayed page.
- Scanned PDFs require OCR before text can be selected.
- PDF.js is loaded from a CDN, so the first load and PDF engine require internet access. The app shell is cached, but full offline PDF operation is not yet guaranteed.
- Keep backups. Safari may clear website storage, and browser storage is not a substitute for a separate backup.

## Run / install
Host the folder on HTTPS (GitHub Pages is one free option). Open the hosted URL in Safari on iPad, then Share -> Add to Home Screen. Enable "Open as Web App" if offered.

For local testing on a computer, serve this folder over localhost rather than opening index.html directly; service workers require HTTPS or localhost.

## Next development milestone
Add true PDF page rendering, robust text-layer selection, multi-page full-text indexing, annotation overlays, and a proper backup restore flow.
