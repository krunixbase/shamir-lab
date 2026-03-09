# Research Notes — Shamir Lab

This document collects research notes, experiment logs, observations, and analytical findings related to Shamir’s Secret Sharing (SSS), reconstruction behavior, fuzzing workflows, and threshold‑based cryptographic analysis.

---

## 1. Purpose

This file serves as a central place for documenting:

- experimental results,
- observations from tests,
- edge‑case behavior,
- anomalies in algorithm performance,
- ideas for further research,
- findings from fuzzing and error analysis.

---

## 2. Experiments

### 2.1 Reconstruction tests below threshold
**Description:**  
Evaluate reconstruction behavior when the number of shares is below the required threshold.

**Results:**  
- Reconstruction fails as expected.  
- Interpolation values show high numerical instability.  
- Near‑modulo values produce inconsistent intermediate results.

**Notes:**  
Potential area for side‑channel or error‑based analysis.

---

### 2.2 Fuzzing the share generator
**Description:**  
Randomized generation of shares with boundary values.

**Results:**  
- Shares near 0 and p‑1 cause more frequent reconstruction anomalies.  
- Larger prime fields reduce instability but increase computation time.

**Notes:**  
Input validation and sanity checks should be strengthened.

---

## 3. Edge Cases for Further Study

- Shares with identical x‑coordinates.  
- Shares generated with incorrect RNG seeds.  
- Reconstruction using non‑prime moduli.  
- Rounding errors in languages without native big‑integer support.  
- Behavior when coefficients are zero or near-zero.

---

## 4. Future Experiment Ideas

- Mutation‑based fuzzing of share sets.  
- Bit‑flip error resistance analysis.  
- Performance benchmarks for varying thresholds.  
- Cross‑language comparison (Python, Rust, C).  
- Automated corpus generation for fuzzing.

---

## 5. General Observations

The lab would benefit from:

- automated dataset generation,  
- continuous fuzzing pipelines,  
- structured reporting of anomalies,  
- reproducible experiment templates.

