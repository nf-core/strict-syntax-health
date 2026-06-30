# Workflow outputs migration: raredisease

- Generated: 2026-06-30T00:40:59.189498+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:843`](https://github.com/nf-core/raredisease/blob/98d93c38f82bf85271793aff4d7839076ec0ad79/main.nf#L843)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/98d93c38f82bf85271793aff4d7839076ec0ad79/conf/base.config#L65) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/98d93c38f82bf85271793aff4d7839076ec0ad79/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
