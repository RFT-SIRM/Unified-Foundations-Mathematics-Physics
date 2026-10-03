# Verification Policy

## Four evidence levels

### Level A — Exact mathematics

Symbolic identities derived from definitions and algebra.

### Level B — Computational verification

Numerical or exhaustive tests that check a defined property over a declared domain.

### Level C — Formal verification

Lean/Mathlib proof accepted by the compiler.

### Level D — Cross-module consequence

A result derived from already established components and independently checked.

## Reporting rule

Every result must state its evidence level.

Examples:

- `EXACT`
- `COMPUTATIONALLY VERIFIED`
- `FORMALLY PROVED`
- `SUPPORTED / OPEN`
- `REJECTED`
- `PROVISIONAL`

## Test archives

Large test archives are retained as supporting evidence. They do not substitute for proof.

Any future large-scale test campaign must include its actual generated artifact, parameters, code version, and execution date.

## Numerical discipline

Use exact arithmetic where feasible.

When floating-point arithmetic is unavoidable:

- state precision;
- state tolerance;
- report maximum absolute and relative errors;
- distinguish roundoff from mathematical error.
