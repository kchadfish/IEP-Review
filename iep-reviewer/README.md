# iep-reviewer

Scaffold for an Embrace-specific IEP review application that keeps PDF parsing in the browser and uses Google Apps Script for the secure review backend.

## Architecture summary

- Parse and inspect Embrace PDFs locally in the browser with PDF.js.
- Normalize extracted content into a shared IEP data contract with evidence and confidence metadata.
- Send normalized findings to Apps Script for applicability, rule evaluation, reporting, and optional Drive integration.
- Use synthetic Embrace student data only; do not commit or process real student PII in this repository.

## Planned scripts

- `npm run build` &mdash; TypeScript project validation
- `npm run lint` &mdash; repository linting once ESLint dependencies are installed
- `npm test` &mdash; placeholder until parser and rule-engine tests are added

## Key docs

- `docs/architecture.md`
- `docs/data-model.md`
- `docs/rule-engine.md`
- `docs/security.md`
- `docs/testing-plan.md`
- `docs/deployment.md`
