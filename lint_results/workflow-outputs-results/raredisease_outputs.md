# Workflow outputs migration: raredisease

- Generated: 2026-10-06T00:23:10.126246+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:1009`](https://github.com/nf-core/raredisease/blob/ad0f46ebfb82677d9e750a8d523d4a5de97a6ade/main.nf#L1009)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/ad0f46ebfb82677d9e750a8d523d4a5de97a6ade/conf/base.config#L68) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/ad0f46ebfb82677d9e750a8d523d4a5de97a6ade/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
