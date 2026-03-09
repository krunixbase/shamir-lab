<p align="center">
  <img src="https://img.shields.io/badge/status-active-brightgreen.svg" alt="Status: Active">
  <img src="https://img.shields.io/badge/project-type%3A%20research-blue.svg" alt="Project Type: Research">
  <img src="https://img.shields.io/badge/language-python%203.10+-yellow.svg" alt="Python 3.10+">
  <img src="https://img.shields.io/badge/license-MIT-lightgrey.svg" alt="License: MIT">
  <img src="https://img.shields.io/badge/security-research%20only-red.svg" alt="Security: Research Only">
  <img src="https://img.shields.io/github/last-commit/krunixbase/shamir-lab.svg" alt="Last Commit">
  <img src="https://img.shields.io/github/repo-size/krunixbase/shamir-lab.svg" alt="Repo Size">
</p>



# shamir‑lab

Laboratory environment for research, cracking experiments, fuzzing workflows, and edge‑case analysis related to Shamir’s Secret Sharing (SSS).
This repository consolidates and unifies two previous research labs:

- Shamir-Cracker-Lab

- shamir_cracker_lab

The goal is to provide a single, coherent workspace for experimentation, algorithmic exploration, forensic workflows, and validation of threshold‑based secret‑sharing schemes.

---

# 🔍 Purpose and Scope

The repository serves as a sandbox for:

- analyzing the behavior of Shamir’s Secret Sharing under adversarial conditions

- exploring brute‑force and near‑threshold cracking strategies

- generating synthetic shares and edge‑case datasets

- building fuzzing harnesses for robustness testing

- performing forensic reconstruction and evidence collection

- validating assumptions used in higher‑level cryptographic systems

It is intentionally experimental and research‑oriented.

---

# 📁 Repository Structure

```
shamir-lab/
│
├── src/
│   ├── analyzer.py
│   ├── brute-force.py
│   ├── generator.py
│   └── utils.py
│
├── forensic-deliverable/
│   ├── ABOUT.txt
│   ├── CONTACT.md
│   ├── README.md
│   ├── evidence/
│   ├── logs/
│   └── reports/
│
├── docs/
│   └── research-notes.md   (optional, for future work)
│
├── README.md
├── LICENSE
└── SECURITY.md
```

## Key directories

- src/ — core cracking tools, generators, analyzers, utilities

- forensic-deliverable/ — structured evidence, logs, and reports for forensic workflows

- docs/ — technical notes, research logs, design documents

---

# 🧪 Core Components

## Cracking & Analysis Tools

- analyzer.py — share inspection, threshold analysis, entropy checks

- brute-force.py — brute‑force reconstruction attempts for research purposes

- generator.py — synthetic share generation for fuzzing and testing

- utils.py — helper functions used across experiments

## Forensic Deliverables

Contains structured materials for documenting experiments, including:

- evidence snapshots

- logs

- forensic reports

- metadata and chain‑of‑custody notes

---

# 🚀 Usage Overview

## Generate test shares

```
bash
python src/generator.py
```

## Run brute‑force experiments

```
bash
python src/brute-force.py
```

## Analyze share sets

```
bash
python src/analyzer.py
```

The tools are intentionally modular so they can be combined into pipelines or fuzzing harnesses.

---

# 🧭 Roadmap

- fuzzing harness for SSS edge‑case discovery

- automated corpus generation

- performance benchmarks for cracking strategies

- integration with shamir-validator

- research notes and experiment templates

- reproducible forensic workflows

---

# 🔒 Security Notice

This repository is intended exclusively for research, validation, and educational purposes.
It must not be used to attack real systems, break confidentiality of legitimate secrets, or bypass security controls.

See SECURITY.md for details.

---

# 📜 License

The repository includes a LICENSE file defining usage terms.
If missing, choose a license consistent with the rest of the krunixbase ecosystem (MIT or Apache‑2.0 are typical for research tools).

---
