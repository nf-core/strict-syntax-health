# Workflow outputs migration: raredisease

- Generated: 2026-07-02T00:40:30.645799+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:990`](https://github.com/nf-core/raredisease/blob/adfc25bcd8532d5c2123dca9c20d3ab5f135f842/main.nf#L990)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/adfc25bcd8532d5c2123dca9c20d3ab5f135f842/conf/base.config#L65) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/adfc25bcd8532d5c2123dca9c20d3ab5f135f842/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
