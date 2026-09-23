# Workflow outputs migration: raredisease

- Generated: 2026-09-23T00:24:00.755370+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:998`](https://github.com/nf-core/raredisease/blob/0943510188a4a48d374d3d781e581c251caf72ba/main.nf#L998)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/0943510188a4a48d374d3d781e581c251caf72ba/conf/base.config#L68) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/0943510188a4a48d374d3d781e581c251caf72ba/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
