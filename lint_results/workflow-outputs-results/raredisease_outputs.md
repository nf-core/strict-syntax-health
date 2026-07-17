# Workflow outputs migration: raredisease

- Generated: 2026-07-17T00:31:28.470891+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:999`](https://github.com/nf-core/raredisease/blob/d185758f85619fcb15eb6b55223171dec6a60a2c/main.nf#L999)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/d185758f85619fcb15eb6b55223171dec6a60a2c/conf/base.config#L65) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/d185758f85619fcb15eb6b55223171dec6a60a2c/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
