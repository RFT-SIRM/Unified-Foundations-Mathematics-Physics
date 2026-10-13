# Scientific Architecture

## Layer 0 — Research environment

UltraCore-RFT provides the laboratory context and surrounding research infrastructure.

## Layer 1 — Mathematical core

Evgeny's Theorem provides the principal current exact result:

$$
\Delta_m(H^4,\theta)=-16(3^{m-1}+1)\sin^2\!\left(\frac{\theta}{2}\right).
$$

This identity is machine-checked in Lean 4 for every $m \ge 1$ and every $\theta$ (concrete SU(2) connection operators on the Sierpiński gasket, fourth moment; evidence level C, see [FORMALIZATION.md](./FORMALIZATION.md)). The Lean statement is the $\Delta_m$ identity; it has not yet been independently peer-reviewed.

## Layer 2 — Operator and symmetry structures

- graph / fractal operators;
- SU(2) edge transport;
- unitary edge matrices;
- connection operators;
- gauge / symmetry transformations;
- trace and spectral constructions.

## Layer 3 — Invariants

- trace defects;
- normalized spectral invariants;
- conservation / accounting identities;
- energy invariants;
- graph scheduling invariants.

## Layer 4 — Spectral and arithmetic structures

Spectra, spectral gaps, scaling laws, arithmetic local factors, transfer operators.

## Layer 5 — Application modules

- Yang–Mills
- Riemann / Hilbert–Pólya
- BSD
- Navier–Stokes
- P vs NP / scheduling
- Phi-Genesis / fractal spectral research

Each module remains independently testable.

## Layer 6 — Verification

- symbolic derivation;
- numerical computation;
- exhaustive testing;
- adversarial testing;
- formal proof;
- reproducibility.

A numerical result is never silently converted into a formal theorem.
