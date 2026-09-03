# Deployment

## Local development

1. Install project dependencies.
2. Build browser and Apps Script artifacts into `dist/`.
3. Copy `clasp.json.example` to `.clasp.json` and add the Apps Script project ID.
4. Deploy with clasp after manifest and scopes are finalized.

## Production notes

- Bundle PDF.js locally.
- Keep browser assets and Apps Script server code separated through the build process.
- Validate school-calendar configuration before enabling service date rules.
