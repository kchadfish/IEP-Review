# Security

## Data handling

- Keep source PDFs local to the browser unless a user explicitly opts into Drive retention.
- Do not send IEP content to third-party OCR or LLM services.
- Use synthetic Embrace data in development, fixtures, and tests.

## Workspace boundaries

- Apps Script handles authentication and domain-scoped access.
- PropertiesService stores configuration only.
- Drive, Docs, and Sheets integrations should be optional and explicitly enabled.

## Review expectations

Districts still need their own FERPA and security review; storing data in Google Workspace alone is not a blanket approval.
