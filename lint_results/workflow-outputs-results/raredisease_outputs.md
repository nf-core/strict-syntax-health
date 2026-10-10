# Workflow outputs migration: raredisease

- Generated: 2026-10-10T00:24:20.171041+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:1017`](https://github.com/nf-core/raredisease/blob/39ed1e17d0d374a6898a7e40fcded818b5783017/main.nf#L1017)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/39ed1e17d0d374a6898a7e40fcded818b5783017/conf/base.config#L68) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/39ed1e17d0d374a6898a7e40fcded818b5783017/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
