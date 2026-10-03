# Unified Foundations — Mathematics & Physics

[![RFT-SIRM](https://img.shields.io/badge/Org-RFT--SIRM-0f172a?style=for-the-badge)](https://github.com/RFT-SIRM)
[![Project](https://img.shields.io/badge/GitHub%20Project-Unified%20Foundations-6366f1?style=for-the-badge)](https://github.com/users/RFT-SIRM/projects/4)
[![Evgeny-Theorem](https://img.shields.io/badge/Core-Evgeny--Theorem-5aa9ff?style=for-the-badge)](https://github.com/RFT-SIRM/Evgeny-Theorem)
[![License](https://img.shields.io/badge/License-Apache%202.0-eab308?style=for-the-badge)](./LICENSE)

**Organization:** RFT-SIRM  
**Laboratory context:** UltraCore-RFT  
**GitHub Project:** [Unified Foundations — Mathematics & Physics](https://github.com/users/RFT-SIRM/projects/4)  
**License:** Apache License 2.0

## Purpose

Cross-repository research program that connects mathematical structures, operator constructions, spectral methods, computational verification, and Lean 4 formalization across several fundamental areas of mathematics and physics.

Common research pattern:

> structure → operator / transition → invariant → spectral or structural constraint → global property → verification

This repository is the **program map and scientific record**. Individual repositories remain independent sources of code, history, and formalization.

## Core identity

$$
\Delta_m(H^4,\theta)=-16(3^{m-1}+1)\sin^2(\theta/2).
$$

At $\theta=\pi/2$:

$$
I_\infty=-\frac{8}{9}.
$$

Evgeny's Theorem is the principal mathematical core. Operator-level Lean formalization is an active workstream. Numerical checks are kept separate from formal proof status.

## Research modules

| Module | Focus |
|--------|--------|
| [Evgeny's Theorem](https://github.com/RFT-SIRM/Evgeny-Theorem) | Exact trace-defect identity on the Sierpiński gasket |
| SU(2) / Operators | Unitary edge transport, connection operators |
| Yang–Mills | Gauge / spectral constructions |
| Riemann / Hilbert–Pólya | Candidate spectral–arithmetic structure |
| BSD | Local SU(2) factors; global rank open |
| Navier–Stokes | Invariant / transition formulation |
| P vs NP / Scheduling | Conflict graphs, bounded execution |
| [Phi-Genesis](https://github.com/RFT-SIRM/Phi-Genesis) | Fractal spectral research |
| [RFT-Cosmology-Genesis](https://github.com/RFT-SIRM/RFT-Cosmology-Genesis) | Phenomenological Pass-1 coupling |
| [RFT-QPU-Sierpinski](https://github.com/RFT-SIRM/RFT-QPU-Sierpinski) | Candidate qubit architecture |
| [RFT-Invariant-Battery.](https://github.com/RFT-SIRM/RFT-Invariant-Battery.) | Energy-system research model |

See [`MODULES.md`](./MODULES.md) and [`PROBLEM_REGISTRY.md`](./PROBLEM_REGISTRY.md).

## Document map

| File | Role |
|------|------|
| [`ARCHITECTURE.md`](./ARCHITECTURE.md) | Layered scientific architecture |
| [`PROJECT_CHARTER.md`](./PROJECT_CHARTER.md) | Charter and objective |
| [`FORMALIZATION.md`](./FORMALIZATION.md) | Lean 4 plan and milestones |
| [`RESEARCH_METHOD.md`](./RESEARCH_METHOD.md) | Hypothesis → verification cycle |
| [`VERIFICATION_POLICY.md`](./VERIFICATION_POLICY.md) | Evidence levels A–D |
| [`RESULT_STATUS.md`](./RESULT_STATUS.md) | Established vs open results |
| [`RESEARCH_RECORD.md`](./RESEARCH_RECORD.md) | Dated program record |
| [`ROADMAP.md`](./ROADMAP.md) | Phased roadmap |
| [`CONTRIBUTING.md`](./CONTRIBUTING.md) | Contribution rules |
| [`PROJECT_SETUP.md`](./PROJECT_SETUP.md) | GitHub Project fields |

## Status vocabulary

- **Verified** — reproduced by the stated procedure  
- **Formally proved** — accepted by the declared Lean toolchain  
- **Supported** — independent checks agree; full proof not established  
- **Rejected** — failed a defined test  
- **Open** — insufficient evidence or missing proof  
- **Provisional** — working result requiring re-verification  

No status is upgraded without a reproducible record. Negative results are first-class.

## Principle

The scientific value of the program is determined by the mathematical results obtained from the framework, not by the project label.

## License

Apache-2.0 — see [`LICENSE`](./LICENSE).
