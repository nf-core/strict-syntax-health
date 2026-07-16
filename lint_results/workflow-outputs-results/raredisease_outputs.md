# Workflow outputs migration: raredisease

- Generated: 2026-07-16T00:29:49.318655+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:996`](https://github.com/nf-core/raredisease/blob/e5dd5bb7203ae46065e93d25f10cca2abdacdfec/main.nf#L996)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/e5dd5bb7203ae46065e93d25f10cca2abdacdfec/conf/base.config#L65) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/e5dd5bb7203ae46065e93d25f10cca2abdacdfec/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
