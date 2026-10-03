# Formalization Plan — Lean 4

## Environment

Primary formalization environment:

- Lean 4
- Mathlib
- current project toolchain: Lean 4.33.1

## Central proof chain

The intended proof chain is:

1. define SU(2) edge rotations;
2. prove their unitarity;
3. construct the connection operator;
4. prove its diagonal;
5. derive the diagonal of \(H^2\);
6. reduce the fourth trace to local contributions;
7. classify the relevant flux/axis contributions;
8. perform the exact combinatorial count;
9. derive the closed form for \(\Delta_m(H^4,\theta)\).

## Current milestone

The formalization already contains:

- `edgeUnitary`;
- `edgeUnitaryWithAxis`;
- `connectionOperator`;
- `connectionOperatorWithAxis`;
- `HC`;
- `HCprime`;
- a proved `connectionOperator_diagonal` identity.

The immediate next mathematical reduction is the diagonal of \(H^2\).

## Formal status rule

A statement is marked formally proved only when the Lean source compiles successfully in the recorded environment without an unproved axiom standing in for the mathematical content of the claim.

A bridge theorem that is merely postulated must be labelled as an assumption, not as a completed proof.
