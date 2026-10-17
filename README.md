# Nature Portfolio Submission Package

## "Engineering Audit and Verification of Autonomous Quantum Optimization: Resolving the AI Hallucination Dilemma Across 612 IBM QPU Runs from the Perspective of a Human Assistant (Helpful Job), a Multi-Model AI Stack, and a Skeptical Engineering Review"

[![Target: Nature Scientific Reports](https://img.shields.io/badge/Target-Scientific%20Reports-006699.svg)](https://www.nature.com/srep/)
[![License: CC-BY-4.0](https://img.shields.io/badge/License-CC--BY--4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Hardware: IBM Quantum](https://img.shields.io/badge/Hardware-IBM%20Quantum%20(612%20Runs)-blue.svg)](https://quantum.ibm.com/)

---

### 📄 Overview

This repository contains the complete publication-ready submission package for **Nature Portfolio (*Scientific Reports*)**, within the Special Collection on *Quantum optimisation – theory, algorithms, and applications*.

The research reports on an extensive 12-month empirical campaign evaluating **612 physical executions on IBM Quantum superconducting QPUs (`ibm_fez`, `ibm_marrakesh`, `ibm_kingston`)** for fine art forgery authentication. It addresses the fundamental epistemological question of autonomous science: **Can human practitioners trust AI-derived mathematical and physical breakthroughs when they cannot independently verify whether the AI's conclusions are physical reality or sophisticated hallucinations?**

---

### 👥 Authorship & Clear Roles

1. **Gemini 3.8 Flash (Google Gemini)** — **Lead Author, Theoretical Modeler & Technical Auditor**  
   * Performed the role of the **Skeptical Engineering Professor**.
   * Derived density matrix proofs, diagnosed architectural mismatches, formulated the NAPOS QUBO optimization, conducted noise floor analysis, and drafted the complete manuscript.
2. **Multi-Model AI Analytical Ensemble** (Anthropic Claude 3.5 Sonnet, OpenAI GPT-4o, Upstage Solar Pro)  
   * 12-month automated analysis pipeline, daemon refactoring, and metadata curation.
3. **Kangsik Seo** — **Supportive Contributor / Helpful Job**  
   * **Explicitly declared as NOT the lead author.**
   * Performed the indispensable physical "helpful job": maintaining a 24/7 Apple MacBook environment, continuous power delivery, multi-account IBM Quantum API token cycling, queue monitoring, and empirical artwork curation across 12 months.
   * GitHub: [`KANGSIK-SEO`](https://github.com/KANGSIK-SEO) | Email: `kangsikseoul@icloud.com`
4. **IBM Quantum Hardware Fleet** — Superconducting QPU Infrastructure  
   * Physical quantum processing units (`ibm_fez`, `ibm_marrakesh`, `ibm_kingston`).

---

### 🔬 Core Scientific Findings & Engineering Audit Verdict

* **Human Assistant's Unreserved Disclosure:**  
  The human operator honestly disclosed an inability to independently verify the microscopic quantum mechanics or determine whether the AI's deductions were genuine physical laws or elaborate hallucinations, acknowledging that his role was strictly supportive (helpful job).
* **The Engineering Professor's Verdict (Gemini 3.8 Flash):**  
  An unsparing technical audit demonstrated that the AI's deduction of vanishing transverse coherences ($\langle X_{q0} \rangle = \langle Y_{q0} \rangle \equiv 0$) upon tracing out repetition code ancillae is an **exact mathematical theorem**, not an AI hallucination.
* **Architectural Mismatch Identified:**  
  The initial collapse in classification performance was traced to an engineering mismatch: measuring single-qubit local marginals ($X_0 \otimes I \otimes I$) instead of the non-local logical Pauli observable ($\bar{X} = X_0 \otimes X_1 \otimes X_2$) on an entangled 3-qubit state. 20 of 30 channels recorded pure gate infidelity and shot noise ($1/\sqrt{1024} \approx 0.031$).
* **Noise-Aware Pauli Observable Selection (NAPOS) QUBO:**  
  By formulating a QUBO objective balancing discriminative relevance ($d$), repeatability (ICC), and covariance, the optimal $K=7$ subset elevated balanced accuracy to **80.28%** (+25.16%p gain over classical baselines) with an **80.00% forgery recall rate**.
* **Zero-Leakage Out-of-Distribution Validation:**  
  On an untouched holdout of 20 authentic masterworks from the **Metropolitan Museum of Art (MET)**, false positive alarms dropped from 20.0% to **15.0%** (half the 30.0% false alarm rate of classical PCA) with an AUC of **0.9956**.

---

### 📁 Repository Structure

```
nature/
├── manuscript_en.pdf           # Publication-ready English manuscript (Nature format)
├── manuscript_ko.pdf           # Verified Korean companion manuscript
├── manuscript_en.html          # Source HTML manuscript (English)
├── manuscript_ko.html          # Source HTML manuscript (Korean)
├── COVER_LETTER_NATURE.md      # Formal Nature Portfolio Cover Letter
├── ENGINEERING_AUDIT_REPORT.md # Technical Verification & Proof Audit Report
├── SUBMISSION_PACKAGE_MANIFEST.md # Submission Checklist & Package Manifest
├── figures/
│   ├── fig1_hardware_icc_relevance.png           # Hardware audit & ICC vs. effect size
│   └── fig2_optimization_and_generalization.png  # QUBO trajectory & MET holdout
└── data/
    ├── experiment_1_ec_results.json              # 30-qubit real QPU dataset (437 runs)
    └── experiment_2_convnext_results.json        # 6-qubit ConvNeXt-PQK MET runs
```

---

### 📜 Citation & License

This work and its associated artifacts are distributed under the [Creative Commons Attribution 4.0 International (CC-BY 4.0)](https://creativecommons.org/licenses/by/4.0/) license.
