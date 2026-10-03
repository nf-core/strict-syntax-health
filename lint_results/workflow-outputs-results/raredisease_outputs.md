# Workflow outputs migration: raredisease

- Generated: 2026-10-03T00:24:40.943906+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:1009`](https://github.com/nf-core/raredisease/blob/c191256e4ce2414d9e95513b5643d850b95003da/main.nf#L1009)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/c191256e4ce2414d9e95513b5643d850b95003da/conf/base.config#L68) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/c191256e4ce2414d9e95513b5643d850b95003da/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
