# Formalization Plan — Lean 4

## Environment

- Lean 4
- Mathlib
- Toolchain as pinned in [Evgeny-Theorem](https://github.com/RFT-SIRM/Evgeny-Theorem) `formalization/`

## Central proof chain

1. define SU(2) edge rotations;
2. prove their unitarity;
3. construct the connection operator;
4. prove its diagonal;
5. derive the diagonal of $H^2$;
6. reduce the fourth trace to local contributions;
7. classify flux / axis contributions;
8. exact combinatorial count;
9. closed form for $\Delta_m(H^4,\theta)$.

## Current milestone

Established in Lean (Evgeny-Theorem):

- graph infrastructure (`SG(m)`, `Vertex`, `Adj`, degree);
- unitarity lemmas;
- base case `traceDefect_one` for $m=1$;
- work on trace expansion $(D-A)^4$, orientation, flipped-face count toward general $m$.

## Formal status rule

A statement is marked formally proved only when the Lean source compiles in the recorded environment without an unproved axiom standing in for the mathematical content of the claim.

A postulated bridge theorem must be labelled as an assumption, not as a completed proof.
