# Research Modules

## 1. Evgeny's Theorem

Fractal/Sierpiński-gasket trace-defect construction.

Principal identity:

\[
\Delta_m(H^4,\theta)
=-16(3^{m-1}+1)\sin^2(\theta/2).
\]

Current focus: complete operator-level Lean proof.

## 2. SU(2) / Operator Layer

Defines the Hilbert-space indexing, Pauli-axis rotations, edge transport, connection operators, and related unitary constructions.

Current formalization work proceeds from unitarity and diagonal identities toward the diagonal of \(H^2\), trace identities, and the final defect formula.

## 3. Yang–Mills

Studies the SU(2) gauge structure, holonomy, continuum scaling, transfer/Hamiltonian constructions, and mass-gap-related questions.

The module records exact local identities separately from the much stronger continuum and quantum-field-theoretic questions.

## 4. Riemann / Hilbert–Pólya

Studies candidate self-adjoint/symmetric spectral constructions and arithmetic trace/prime-orbit structures.

The module records both successful structural matches and mismatches.

## 5. BSD

Uses the exact local SU(2) representation associated with elliptic-curve Frobenius data:

\[
\cos\theta_p=\frac{a_p}{2\sqrt p},
\qquad
U_p=\operatorname{diag}(e^{i\theta_p},e^{-i\theta_p}).
\]

The global rank relation remains a separate open problem.

## 6. Navier–Stokes

Studies the invariant/transition structure of incompressible flow, especially energy balance and divergence-free constraints.

Numerical diagnostics are kept distinct from regularity or global existence proofs.

## 7. P vs NP / Scheduling

Models transaction conflicts as graph structure and studies admissibility, bounded execution, invariants, and combinatorial complexity.

The scheduler module is an application of the framework to a concrete computational problem, not a claim that P vs NP has been resolved.

## 8. Phi-Genesis / Fractal Spectral Module

Studies spectral decimation, fractal Weyl behavior, gaps, twists, and candidate fermion-mass selection structures on the Sierpiński gasket and related systems.

Verified, rejected, and unresolved claims are preserved separately.
