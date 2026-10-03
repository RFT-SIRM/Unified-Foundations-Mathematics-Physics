# Result Status Ledger

## Established mathematical results

### Evgeny's Theorem — exact formula

\[
\Delta_m(H^4,\theta)
=-16(3^{m-1}+1)\sin^2(\theta/2).
\]

At \(\theta=\pi/2\):

\[
I_\infty=-\frac89.
\]

### Local BSD SU(2) identity

For an elliptic curve over \(\mathbb{Q}\):

\[
a_p=p+1-\#E(\mathbb F_p),
\qquad
\cos\theta_p=\frac{a_p}{2\sqrt p}.
\]

With

\[
U_p=\operatorname{diag}(e^{i\theta_p},e^{-i\theta_p}),
\]

the local Euler factor is represented exactly through the corresponding SU(2) matrix expression.

## Formalization status

The operator formalization is active. The diagonal identity

\[
H_{uu}=\deg(u)
\]

has been proved in the current Lean development.

The next target is the general diagonal formula for \(H^2\), followed by the fourth-trace reduction and final combinatorial identity.

## Mixed / open results

Other modules contain computational evidence, failed hypotheses, and open constructions. Their individual status is recorded in module-specific documents.

## Important recordkeeping rule

Do not report a historical numerical run as a newly executed run unless its actual artifact is available and its execution can be independently established.
