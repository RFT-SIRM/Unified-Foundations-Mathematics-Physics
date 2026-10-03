# Contributing to the Research Record

## Rule 1 — Reproducibility

Every nontrivial computational claim must be reproducible.

## Rule 2 — No silent upgrades

Do not change `open` to `verified`, or `verified` to `proved`, without evidence supporting the new status.

## Rule 3 — Preserve failed hypotheses

Do not delete a failed experiment merely because a newer hypothesis replaced it.

## Rule 4 — Separate layers

Keep distinct:

- definitions;
- exact mathematics;
- numerical evidence;
- formal proof;
- interpretation.

## Rule 5 — Record environment

Include:

- language/tool version;
- dependencies;
- commit hash;
- operating environment where relevant;
- command used to reproduce the result.

## Rule 6 — Small claims first

A module should establish local identities before making global claims.

## Rule 7 — Formalization

Lean files should compile from a clean checkout with the declared toolchain.
