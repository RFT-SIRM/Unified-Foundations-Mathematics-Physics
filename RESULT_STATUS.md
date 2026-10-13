# Result Status Ledger

## Established mathematical results

### Evgeny's Theorem — exact formula

$$
\Delta_m(H^4,\theta)=-16(3^{m-1}+1)\sin^2\!\left(\frac{\theta}{2}\right).
$$

At $\theta=\pi/2$:

$$
I_\infty=-\frac{8}{9}.
$$

Evidence levels: A (exact) and C (`FORMALLY PROVED` in Lean 4 for every $m \ge 1$, fourth moment; see [FORMALIZATION.md](./FORMALIZATION.md)). The value $I_\infty$ is a consequence of the formula; it is not part of the statement `traceDefect_closed`.

### Local BSD SU(2) identity

For an elliptic curve over $\mathbb{Q}$:

$$
a_p = p + 1 - \lvert E(\mathbb{F}_p)\rvert,
\qquad
\cos\theta_p = \frac{a_p}{2\sqrt{p}}.
$$

With

$$
U_p = \mathrm{diag}(e^{i\theta_p}, e^{-i\theta_p}),
$$

the local Euler factor is represented exactly through the corresponding SU(2) matrix expression.

## Formalization status

`FORMALLY PROVED`: $\Delta_m(H^4,\theta)=-16(3^{m-1}+1)\sin^2(\theta/2)$ for every $m \ge 1$ and every $\theta$, in the Lean 4 development ([Evgeny-Theorem](https://github.com/RFT-SIRM/Evgeny-Theorem), theorem `traceDefect_closed`; no `sorry`, standard axioms only). Details and reproduction: [FORMALIZATION.md](./FORMALIZATION.md).

Not covered: $m = 0$; moments other than the fourth; independent review that the Lean definitions of the operators match the intended objects.

## Mixed / open results

Other modules contain computational evidence, failed hypotheses, and open constructions. Status is recorded in module-specific documents and in [PROBLEM_REGISTRY.md](./PROBLEM_REGISTRY.md).

## Recordkeeping rule

Do not report a historical numerical run as a newly executed run unless its artifact is available and execution can be independently established.
