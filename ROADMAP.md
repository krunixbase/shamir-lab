# Roadmap — Shamir Lab

This roadmap outlines the planned development, research directions, and long‑term goals for the *shamir‑lab* project.  
The lab focuses on experimentation, cryptographic analysis, fuzzing workflows, and forensic reconstruction related to Shamir’s Secret Sharing (SSS).

---

## 1. Core Objectives

- Provide a unified research environment for analyzing SSS behavior.
- Develop tools for cracking, reconstruction, and fuzzing.
- Build reproducible forensic workflows.
- Explore edge‑case behavior and algorithmic weaknesses.
- Support cross‑language and cross‑implementation comparisons.

---

## 2. Short‑Term Goals (0–3 months)

### 🔹 2.1 Codebase Enhancements
- Refactor core modules for clarity and modularity.
- Add type hints and improve documentation across `src/`.
- Introduce consistent logging across all tools.
- Expand `utils.py` with reusable math and GF(p) helpers.

### 🔹 2.2 Research Infrastructure
- Extend `research-notes.md` with experiment templates.
- Add reproducible experiment scripts (e.g., `experiments/` directory).
- Create datasets for fuzzing and reconstruction testing.

### 🔹 2.3 Forensic Deliverables
- Standardize structure of `forensic-deliverable/`.
- Add templates for forensic reports and chain‑of‑custody notes.
- Improve evidence collection automation.

---

## 3. Mid‑Term Goals (3–9 months)

### 🔹 3.1 Fuzzing Framework
- Implement mutation‑based fuzzing for share sets.
- Add corpus generation tools for edge‑case exploration.
- Integrate coverage‑guided fuzzing (e.g., AFL‑style workflows).
- Automate detection of anomalies in reconstruction.

### 🔹 3.2 Algorithmic Analysis
- Benchmark reconstruction performance for varying thresholds.
- Analyze behavior under non‑prime moduli.
- Study numerical instability in interpolation.
- Explore side‑channel‑like leakage from reconstruction errors.

### 🔹 3.3 Cross‑Language Implementations
- Add reference implementations in Rust and C.
- Compare performance and correctness across languages.
- Build compatibility tests for share formats.

---

## 4. Long‑Term Goals (9–18 months)

### 🔹 4.1 Advanced Cryptographic Research
- Investigate threshold cryptography beyond SSS (e.g., Feldman, Pedersen).
- Explore verifiable secret sharing (VSS) extensions.
- Study multi‑party computation (MPC) interactions with SSS.

### 🔹 4.2 Tooling and Automation
- Build a full CI pipeline for testing, linting, and reproducibility.
- Add automated report generation for experiments.
- Provide a CLI interface for all core tools.

### 🔹 4.3 Documentation and Knowledge Base
- Expand documentation into a structured knowledge hub.
- Add diagrams, architecture overviews, and math explanations.
- Publish research findings and experiment summaries.

---

## 5. Stretch Goals (Future / Optional)

- Web‑based visualization of shares and reconstruction curves.
- Interactive notebook environment (Jupyter or Quarto).
- Integration with external cryptographic libraries.
- Support for distributed experiments and cluster execution.
- Machine‑learning‑assisted anomaly detection in fuzzing outputs.

---

## 6. Milestones Overview

| Milestone | Target | Description |
|----------|---------|-------------|
| **M1** | Q2 2026 | Core refactor, documentation, experiment templates |
| **M2** | Q3 2026 | Fuzzing framework + dataset generation |
| **M3** | Q4 2026 | Cross‑language implementations + benchmarks |
| **M4** | Q1 2027 | Advanced cryptographic extensions (VSS, MPC) |
| **M5** | Q2 2027 | Full automation, CI, reproducible research suite |

---

## 7. Guiding Principles

- Research‑first: prioritize exploration and understanding.
- Reproducibility: every experiment should be repeatable.
- Transparency: document assumptions, failures, and anomalies.
- Ethics: restrict usage to lawful and responsible research.
- Modularity: tools should be composable and language‑agnostic.

