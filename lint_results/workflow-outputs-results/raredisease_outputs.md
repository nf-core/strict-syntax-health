# Workflow outputs migration: raredisease

- Generated: 2026-10-07T00:23:18.425601+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:1009`](https://github.com/nf-core/raredisease/blob/a681fda5b603a8b942f4f1d1f8feaa3dbbb7b6be/main.nf#L1009)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/a681fda5b603a8b942f4f1d1f8feaa3dbbb7b6be/conf/base.config#L68) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/a681fda5b603a8b942f4f1d1f8feaa3dbbb7b6be/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
