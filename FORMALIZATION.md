# Formalization — Lean 4 (plan and status)

## Environment

- Lean 4
- Mathlib
- Toolchain as pinned in [Evgeny-Theorem](https://github.com/RFT-SIRM/Evgeny-Theorem) (`lean-toolchain` and `lake-manifest.json` in the repository root; Lean sources under `formalization/`)

## Status

**Complete for the stated scope.** `traceDefect_closed` ([`TildeEntries.lean`](https://github.com/RFT-SIRM/Evgeny-Theorem/blob/main/formalization/EvgenyTheorem/TildeEntries.lean)) proves, for every $m \ge 1$ and every $\theta$ and for the concrete SU(2) connection operators on the Sierpiński gasket graph $SG(m)$:

$$
\Delta_m(H^4,\theta)=-16(3^{m-1}+1)\sin^2\!\left(\frac{\theta}{2}\right).
$$

Evidence level C ([VERIFICATION_POLICY.md](./VERIFICATION_POLICY.md)): `FORMALLY PROVED`. No `sorry`; `#print axioms` reports only `propext`, `Classical.choice`, `Quot.sound`. A build from a fresh clone of Evgeny-Theorem completed successfully (state recorded at commit `9ed32ae`).

Scope limits: fourth moment only; $m \ge 1$ (not $m = 0$); the limit value $I_\infty$ is not part of the machine-checked statement; independent review that the Lean definitions match the intended objects has not yet been done.

Reproduce: clone [Evgeny-Theorem](https://github.com/RFT-SIRM/Evgeny-Theorem), then `lake exe cache get && lake build`, and check `#print axioms EvgenyTheorem.traceDefect_closed`.

## Proof route as formalized

1. SU(2) edge rotations and their unitarity; the connection operator and its diagonal; the diagonal of $H^2$.
2. Base cases: $m = 1$ (`traceDefect_one`) and the same case with the corner flux edge reversed (`tilde_base`).
3. Gluing: the level-$(m+1)$ operator is assembled from three copies of the level-$m$ operator; the corner conditions are proved for every $m$ (`sgK_corner_data`).
4. Coupled recursion over two edge orientations, $D_{m+1} = 2D_m + \tilde D_m$ and $\tilde D_{m+1} = D_m + 2\tilde D_m$ (`defect_succ_num`, `defect_succ_til`), then induction to the closed form.

The original plan (diagonal of $H^2$, local reduction of the fourth trace, flux/axis classification, exact combinatorial count) was superseded after step 1: the general case follows the gluing route above.

## Formal status rule

A statement is marked formally proved only when the Lean source compiles in the recorded environment without an unproved axiom standing in for the mathematical content of the claim.

A postulated bridge theorem must be labelled as an assumption, not as a completed proof.
