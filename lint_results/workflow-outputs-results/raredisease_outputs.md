# Workflow outputs migration: raredisease

- Generated: 2026-11-28T00:13:40.469530+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:1036`](https://github.com/nf-core/raredisease/blob/094d1404d0397499f19aabd5c129c137ba8e707a/main.nf#L1036)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/094d1404d0397499f19aabd5c129c137ba8e707a/conf/base.config#L67) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/094d1404d0397499f19aabd5c129c137ba8e707a/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
