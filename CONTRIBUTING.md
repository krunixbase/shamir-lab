# Contributing Guidelines — Shamir Lab

Thank you for your interest in contributing to *shamir‑lab*.  
This document outlines the standards and expectations for contributions to maintain clarity, quality, and consistency across the project.

---

## 1. Workflow

- Each change should be made in a dedicated branch.
- Branch names should follow a clear convention:
  - `feat/...` — new features
  - `fix/...` — bug fixes
  - `refactor/...` — structural improvements
  - `docs/...` — documentation updates
  - `research/...` — experiments, notes, or analysis

---

## 2. Commit Style

This project follows **Conventional Commits**:

- `feat:` — new functionality  
- `fix:` — bug fix  
- `docs:` — documentation changes  
- `refactor:` — internal code changes without altering behavior  
- `test:` — tests  
- `chore:` — maintenance tasks  

**Examples:**

```
feat(generator): add support for large prime fields
fix(analyzer): correct interpolation edge-case handling
docs(research): add fuzzing results for threshold t=5
```

---

## 3. Code Style

- Python code should follow PEP8 and include type hints.
- Functions must include docstrings.
- Code should be modular and testable.
- Avoid duplication; use shared utilities where possible.

---

## 4. Testing

- Every new feature should include unit tests.
- Edge‑case testing is strongly encouraged.
- Fuzzing should be isolated from deterministic tests.

---

## 5. Pull Requests

A PR should include:

- a clear description of the change,
- justification or motivation,
- test results,
- notes on potential side effects.

PRs without tests may be rejected.

---

## 6. Documentation Requirements

Changes affecting functionality should update:

- `README.md` (usage or structure changes),
- `docs/research-notes.md` (research‑related updates),
- `forensic-deliverable/` (if new artifacts are generated).

---

## 7. Security Considerations

Changes involving cryptographic logic must be:

- well‑documented,
- justified,
- aligned with best practices,
- free from security regressions.

---
