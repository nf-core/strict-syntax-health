# Workflow outputs migration: raredisease

- Generated: 2026-08-06T00:28:40.125913+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:1035`](https://github.com/nf-core/raredisease/blob/b2734100ecbbd1507f5f695f1ac22328c225b336/main.nf#L1035)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/b2734100ecbbd1507f5f695f1ac22328c225b336/conf/base.config#L65) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/b2734100ecbbd1507f5f695f1ac22328c225b336/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
