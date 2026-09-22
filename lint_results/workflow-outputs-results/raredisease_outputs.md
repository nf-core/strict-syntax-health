# Workflow outputs migration: raredisease

- Generated: 2026-09-22T00:23:09.327253+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:998`](https://github.com/nf-core/raredisease/blob/6de800bb9fdd96a48210452ff59623b5a298b38c/main.nf#L998)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/6de800bb9fdd96a48210452ff59623b5a298b38c/conf/base.config#L68) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/6de800bb9fdd96a48210452ff59623b5a298b38c/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
