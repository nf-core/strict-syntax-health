# Workflow outputs migration: raredisease

- Generated: 2026-08-12T00:23:01.306504+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:998`](https://github.com/nf-core/raredisease/blob/54b3f0eb4c1f3a5b0409e0e376b8e350003d404c/main.nf#L998)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/54b3f0eb4c1f3a5b0409e0e376b8e350003d404c/conf/base.config#L65) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/54b3f0eb4c1f3a5b0409e0e376b8e350003d404c/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
