# Architecture

The production design is a browser-first PDF extraction pipeline paired with a Google Apps Script review backend.

## Core flow

1. Load Embrace PDFs locally with PDF.js.
2. Extract text, coordinates, rendered page imagery, and checkbox evidence in the browser.
3. Normalize the result into a shared IEP JSON contract.
4. Send normalized findings to Apps Script with `google.script.run`.
5. Run applicability, compliance, cross-section, and heuristic review engines server-side.
6. Return findings with evidence, confidence, and review status to the UI.

## Architectural decisions

- PDF parsing stays in the browser because the forms are not dependable fillable PDFs.
- Apps Script handles authentication, configuration, reporting, Drive integration, and calendars.
- Parser logic is form/version specific so Embrace template drift can be detected instead of silently misparsed.
- Evidence objects are part of the core data model so every finding can be traced back to source pages and bounding boxes.
