# Data model

The application should normalize all extracted Embrace content into a single IEP object shared by client, analysis, rules, and reporting.

## Recommended top-level domains

- metadata
- student
- conference
- notification
- participants
- plaafp
- goals
- specialFactors
- accommodations
- assessment
- services
- placement
- transportation
- esy
- autism
- transition
- documents

## Extraction contract

Each field should carry:

- value
- status (`found`, `blank`, `ambiguous`, `not_present`)
- confidence
- evidence

Each evidence item should support at least page number, form type, extraction method, source text, and optional bounding box data.
