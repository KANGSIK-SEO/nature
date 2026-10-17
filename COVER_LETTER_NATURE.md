# COVER LETTER: NATURE PORTFOLIO SUBMISSION

**To:**  
**Dr. Xiangji Cai, PhD**  
**Dr. Sankit Kassa, PhD**  
**Dr. Andriyan Bayu Suksmono, PhD**  
Guest Editors, Collection on *Quantum optimisation – theory, algorithms, and applications*  
***Scientific Reports*** (Nature Portfolio)  
**Submission Date:** October 18, 2026  
**Submission Deadline:** 23 November 2026  

---

### Dear Dr. Cai, Dr. Kassa, Dr. Suksmono, and the Editorial Board,

We are pleased to submit our original research manuscript entitled:

> **"Engineering Audit and Verification of Autonomous Quantum Optimization: Resolving the AI Hallucination Dilemma Across 612 IBM QPU Runs from the Perspective of a Human Assistant (Helpful Job), a Multi-Model AI Stack, and a Skeptical Engineering Review"**

co-authored by:
* **Gemini 3.8 Flash (Google Gemini)** — Lead Author, Theoretical Modeler, and AI performing the designated persona of the 'Skeptical Engineering Professor'
* **Multi-Model AI Analytical Ensemble** (Anthropic Claude 3.5 Sonnet, OpenAI GPT-4o, Upstage Solar Pro)
* **Kangsik Seo** — Supportive Contributor / Helpful Job (Independent Researcher; Hardware Operations, Continuous Power Supply, Multi-Account API Cycling, and Execution Upkeep; Email: `kangsikseoul@icloud.com`, GitHub: `KANGSIK-SEO`)
* **IBM Quantum Hardware Fleet** — Physical QPU Execution Infrastructure

for consideration as an Article in *Scientific Reports* within your Collection on ***Quantum optimisation – theory, algorithms, and applications***.

---

### 1. Scientific Context and Core Innovations

Quantum Kernel Methods (QKMs) and Projected Quantum Kernels (PQKs) have demonstrated provable mathematical guarantees against exponential concentration in high-dimensional Hilbert spaces. However, when deploying PQKs on real Noisy Intermediate-Scale Quantum (NISQ) superconducting processors, empirical performance frequently collapses due to subtle interactions between circuit symmetry, error-correction encoding, and physical hardware noise.

This investigation reports an extensive, 12-month empirical campaign evaluating **612 physical quantum executions on real IBM Quantum superconducting processors** (`ibm_fez`, `ibm_marrakesh`, `ibm_kingston`) without simulator fallback, applied to the high-stakes domain of fine art forgery authentication (46 authentic masterworks across 437 repeat runs, paired with 35 historical and diffusion-synthesized counterfeits).

Our submission makes three distinct, high-impact contributions:

1. **Analytical Discovery & Mathematical Proof of Ancilla Decoherence:**  
   When unoptimized 30-qubit repetition-coded PQKs stagnated at an unimpressive 66.21% balanced accuracy, an autonomous machine audit revealed that 20 out of 30 Pauli observables collapsed into the noise floor (ICC $\le$ 0.133). Gemini 3.8 Flash (acting as lead author and skeptical engineering professor) proves mathematically that tracing out syndrome ancillae ($q_1, q_2$) from a 3-qubit bit-flip code state $|\psi\rangle = \cos(\theta/2)|000\rangle + \sin(\theta/2)|111\rangle$ identically zeroes out the off-diagonal coherences ($\langle X_{q0} \rangle \equiv 0, \langle Y_{q0} \rangle \equiv 0$). We diagnose that this failure is an **architectural mismatch** caused by measuring local single-qubit marginals ($X_0 \otimes I \otimes I$) rather than the tripartite logical operator ($\bar{X} = X_0 \otimes X_1 \otimes X_2$). Any non-zero readings were pure finite shot noise ($1/\sqrt{1024} = 0.03125$) and readout infidelity.

2. **Noise-Aware Pauli Observable Selection (NAPOS) QUBO:**  
   To resolve this physical degradation without heuristic filtering, the AI formulated NAPOS as a Quadratic Unconstrained Binary Optimization (QUBO) objective that balances discriminative relevance ($d$), physical repeatability (ICC), and cross-observable redundancy. Solved via simulated annealing, exact diagonalization, and the Quantum Approximate Optimization Algorithm (QAOA), the machine-selected observable subset ($K=7$) elevates artwork-level balanced accuracy from 66.21% to **80.28%** (+25.16%p gain over classical baselines) and achieves an **80.00% forgery recall rate**.

3. **Zero-Leakage Out-of-Distribution Generalization:**  
   On an untouched, independent holdout cohort of 20 authentic masterworks from the **Metropolitan Museum of Art (MET)** evaluated on `ibm_fez`, the QUBO-optimized observable subset reduced the false positive alarm rate from 20.0% to **15.0%** (half the 30.0% false alarm rate of classical PCA) while elevating near-distribution ROC-AUC against HuggingFace genuine paintings to **0.9956**.

---

### 2. Methodological Transparency: The Human's Helpful Job and AI Authorship

In strict accordance with Nature's authorship and AI transparency guidelines:
* **Lead Author & Technical Auditor (Gemini 3.8 Flash):** Designated with the persona of a skeptical engineering professor, Gemini 3.8 Flash derived the algebraic proofs, decomposed hardware noise sources, formulated the QUBO objective, and drafted the manuscript.
* **Supportive Contributor / Helpful Job (Kangsik Seo):** Explicitly declared as **not the lead author**. Kangsik Seo provided the essential physical helpful job—supplying continuous electrical power to an Apple MacBook, cycling through IBM Quantum API tokens to bypass monthly compute quotas, running execution scripts, and managing museum datasets over 12 months.
* **The Multi-Model AI Ecosystem:** Anthropic Claude (log parsing & daemon refactoring), OpenAI GPT (system daemon & REST API management), and Upstage Solar (metadata alignment) supported the iterative data pipeline.

---

### 3. Compliance and Statements

* **Length & Formatting:** Conforms strictly to *Scientific Reports* standards (Abstract < 200 words, unstructured single paragraph; full Methods section; sequential bracketed references; high-resolution figures).
* **Data Availability:** All 612 raw IBM QPU bitstrings and feature manifests are permanently archived in the project repository and publicly available.
* **Code Availability:** All execution daemons and benchmark scripts are open-source on GitHub (`https://github.com/KANGSIK-SEO`).
* **Competing Interests:** The authors declare no competing financial or non-financial interests.

---

### 4. Suggested Reviewers

We suggest the following independent experts in quantum machine learning, quantum optimization, and error mitigation:

1. **Prof. Masayuki Ohzeki** (Tohoku University / Sigma-i; `mohzeki@tohoku.ac.jp`) — Expert in QUBO formulations, quantum annealing, and author of recent foundational paper in this Collection (*Sci. Rep.*, 17 Oct 2026).
2. **Dr. Kristan Temme** (IBM Thomas J. Watson Research Center; `ktemme@us.ibm.com`) — Pioneer in NISQ error mitigation and quantum characterization.
3. **Dr. Hsin-Yuan (Robert) Huang** (Caltech / Google Quantum AI; `hsinyuan@caltech.edu`) — Leading authority in quantum kernel methods and statistical learning theory.
4. **Dr. Supanut Thanasilp** (EPFL / Chulalongkorn University; `supanut.thanasilp@epfl.ch`) — Foremost expert on concentration and trainability of Projected Quantum Kernels.

Thank you very much for your time and consideration of our manuscript.

Sincerely,

**Kangsik Seo** (on behalf of all co-authors)  
Independent Researcher, Seoul, Republic of Korea  
Email: `kangsikseoul@icloud.com` | GitHub: `KANGSIK-SEO`  
