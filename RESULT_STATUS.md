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

### Local BSD SU(2) identity

For an elliptic curve over $\mathbb{Q}$:

$$
a_p = p + 1 - \#E(\mathbb{F}_p),
\qquad
\cos\theta_p = \frac{a_p}{2\sqrt{p}}.
$$

With

$$
U_p = \mathrm{diag}(e^{i\theta_p}, e^{-i\theta_p}),
$$

the local Euler factor is represented exactly through the corresponding SU(2) matrix expression.

## Formalization status

Operator formalization is active. The diagonal identity

$$
H_{uu}=\deg(u)
$$

has been proved in the current Lean development. Base case $m=1$ for the trace defect is established in Lean.

Next targets: general $m$, orientation handling, $H^2$ diagonal, fourth-trace reduction, closed combinatorial identity.

## Mixed / open results

Other modules contain computational evidence, failed hypotheses, and open constructions. Status is recorded in module-specific documents and in [PROBLEM_REGISTRY.md](./PROBLEM_REGISTRY.md).

## Recordkeeping rule

Do not report a historical numerical run as a newly executed run unless its artifact is available and execution can be independently established.
