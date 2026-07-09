# Workflow outputs migration: raredisease

- Generated: 2026-07-09T00:34:25.360493+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:996`](https://github.com/nf-core/raredisease/blob/a942e2311f05534ddea21eaaba4ef979ab5f7882/main.nf#L996)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/a942e2311f05534ddea21eaaba4ef979ab5f7882/conf/base.config#L65) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/a942e2311f05534ddea21eaaba4ef979ab5f7882/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
