# AGENTS.md

## Repository guardrails

- Keep source PDF parsing in the browser; do not move that responsibility into Apps Script.
- Treat evidence, confidence, and applicability as first-class concepts in both parser and rule-engine work.
- Use only synthetic Embrace student data in fixtures, examples, tests, and screenshots.
- Prefer small, form-specific parser additions over broad regex-only extraction.
