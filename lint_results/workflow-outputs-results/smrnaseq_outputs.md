# Workflow outputs migration: smrnaseq

- Generated: 2026-11-27T00:14:51.614733+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:246`](https://github.com/nf-core/smrnaseq/blob/b17036c7834fccb3d9c872aca6c92adcefec8298/main.nf#L246)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/smrnaseq/blob/b17036c7834fccb3d9c872aca6c92adcefec8298/conf/modules.config#L192) — 1 reference
- [`tests/strand_orientation/main.nf`](https://github.com/nf-core/smrnaseq/blob/b17036c7834fccb3d9c872aca6c92adcefec8298/tests/strand_orientation/main.nf#L17) — 1 reference
