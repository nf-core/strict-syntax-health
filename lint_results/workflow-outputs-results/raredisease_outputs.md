# Workflow outputs migration: raredisease

- Generated: 2026-10-14T00:21:23.478417+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:1030`](https://github.com/nf-core/raredisease/blob/42a1de1ceaf119df142d3369926dc5f6e30c78e2/main.nf#L1030)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/42a1de1ceaf119df142d3369926dc5f6e30c78e2/conf/base.config#L68) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/42a1de1ceaf119df142d3369926dc5f6e30c78e2/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
