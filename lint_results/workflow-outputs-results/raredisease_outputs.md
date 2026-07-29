# Workflow outputs migration: raredisease

- Generated: 2026-07-29T00:30:53.468111+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:1032`](https://github.com/nf-core/raredisease/blob/b75ae38dc96fbee6bf1b74e7749d7d0131ef485d/main.nf#L1032)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/b75ae38dc96fbee6bf1b74e7749d7d0131ef485d/conf/base.config#L65) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/b75ae38dc96fbee6bf1b74e7749d7d0131ef485d/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
