# Security Policy — Shamir Lab

*shamir‑lab* is a research environment for analyzing, testing, and experimenting with Shamir’s Secret Sharing (SSS).  
It is not intended for production use or for attacking real systems.

---

## 1. Scope of Responsibility

- The project is intended solely for research, education, and algorithm validation.
- The authors are not responsible for misuse of the tools.
- The repository does not provide implementations intended for compromising real systems.

---

## 2. Reporting Security Issues

If you discover:

- a vulnerability,
- a logical flaw,
- an incorrect implementation,
- or a cryptographic weakness,

please report it via:

- GitHub Issues (tagged `security`), or  
- private contact listed in `forensic-deliverable/CONTACT.md`.

---

## 3. Responsible Disclosure

- Do not publish exploits in Issues.  
- Do not share data that could reconstruct real secrets.  
- Do not upload sensitive keys, passwords, or confidential material.

---

## 4. Prohibited Uses

The tools in this repository must not be used for:

- breaking real systems,  
- reconstructing secrets without authorization,  
- bypassing security controls,  
- any activity that violates law or ethics.

---

## 5. Security Recommendations

- Use isolated environments (virtualenv, Docker).  
- Do not test with production data.  
- Apply resource limits when fuzzing.  
- Document anomalies and findings in `docs/research-notes.md`.

