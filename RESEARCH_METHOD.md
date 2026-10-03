# Research Method

## Standard cycle

Each research claim follows:

\[
\boxed{
\text{hypothesis}
\rightarrow
\text{definition}
\rightarrow
\text{derivation}
\rightarrow
\text{code}
\rightarrow
\text{exhaustive/adversarial test}
\rightarrow
\text{confirmation or rejection}
\rightarrow
\text{formalization}
\rightarrow
\text{open problem}
}
\]

Not every claim reaches every stage.

## Required record

For every computational result, record:

- source file;
- commit hash;
- environment;
- parameter range;
- random seed(s), if any;
- number of cases;
- tolerance;
- exact pass/fail rule;
- observed extrema;
- output artifact.

## Negative results

A failed hypothesis is preserved when the test is reproducible. The record must state:

- the original hypothesis;
- the test;
- the observed counterexample or failure;
- the conclusion;
- whether a revised hypothesis remains open.

## Independence

Whenever possible, controls should be included:

- commuting vs non-commuting;
- original vs randomized/gauge-transformed;
- exact vs floating-point;
- finite-level vs asymptotic;
- baseline algorithm vs proposed algorithm.

## Reproducibility

A result is considered reproducible only when another run can be performed from the recorded inputs and produces the stated acceptance result within the declared tolerance.
