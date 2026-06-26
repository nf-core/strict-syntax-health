# Workflow outputs migration: raredisease

- Generated: 2026-06-26T00:44:24.175502+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:821`](https://github.com/nf-core/raredisease/blob/cbb21fff48b6362a7d1fb5de4aa5eae98ca0c221/main.nf#L821)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/cbb21fff48b6362a7d1fb5de4aa5eae98ca0c221/conf/base.config#L65) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/cbb21fff48b6362a7d1fb5de4aa5eae98ca0c221/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
