# Workflow outputs migration: raredisease

- Generated: 2026-06-23T00:43:50.419664+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:798`](https://github.com/nf-core/raredisease/blob/7bf2a9eb68bb69e1012e3b0ecf74666905626669/main.nf#L798)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/7bf2a9eb68bb69e1012e3b0ecf74666905626669/conf/base.config#L65) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/7bf2a9eb68bb69e1012e3b0ecf74666905626669/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
