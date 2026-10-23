# Workflow outputs migration: raredisease

- Generated: 2026-10-23T00:20:49.787856+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:1034`](https://github.com/nf-core/raredisease/blob/7e6599d70339ed382add9eb575d74084f5aeb9fe/main.nf#L1034)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/7e6599d70339ed382add9eb575d74084f5aeb9fe/conf/base.config#L68) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/7e6599d70339ed382add9eb575d74084f5aeb9fe/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
