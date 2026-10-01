# Workflow outputs migration: raredisease

- Generated: 2026-10-01T00:26:48.292524+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:1005`](https://github.com/nf-core/raredisease/blob/6bc345389b3f17149db7c8a47384212c93291e7d/main.nf#L1005)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/6bc345389b3f17149db7c8a47384212c93291e7d/conf/base.config#L68) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/6bc345389b3f17149db7c8a47384212c93291e7d/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
