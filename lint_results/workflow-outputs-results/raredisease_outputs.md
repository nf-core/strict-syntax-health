# Workflow outputs migration: raredisease

- Generated: 2026-10-15T00:21:38.193171+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:1032`](https://github.com/nf-core/raredisease/blob/f071ee24bf49f0f4a504474f75a6916728d2298e/main.nf#L1032)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/f071ee24bf49f0f4a504474f75a6916728d2298e/conf/base.config#L68) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/f071ee24bf49f0f4a504474f75a6916728d2298e/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
