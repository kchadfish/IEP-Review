# Rule engine

Parsing and compliance evaluation must remain separate concerns.

## Pipeline

1. Applicability engine decides which rules are in scope.
2. Deterministic ISBE rules evaluate structured fields.
3. Cross-section consistency checks compare sections and forms.
4. Heuristic analyzers flag issues that need reviewer judgment.
5. Aggregation produces PASS, ISSUE, REVIEW, N/A, or PARSE ERROR outcomes.

## Rule classes

- Presence
- Calculation
- Consistency
- Semantic heuristic
- Professional judgment

Transition, autism, linguistic supports, ESY, and other triggered sections should be modeled as applicability-driven rule sets instead of ad hoc conditionals.
