# Workflow outputs migration: raredisease

- Generated: 2026-10-13T00:27:50.520732+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:1019`](https://github.com/nf-core/raredisease/blob/f633d247442069c0595dc372d59795a81b26d8ea/main.nf#L1019)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/f633d247442069c0595dc372d59795a81b26d8ea/conf/base.config#L68) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/f633d247442069c0595dc372d59795a81b26d8ea/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
