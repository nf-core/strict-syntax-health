# Workflow outputs migration: raredisease

- Generated: 2026-07-03T00:35:08.367630+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:995`](https://github.com/nf-core/raredisease/blob/4ff88ed06dbb90c656d681a10488520addebd47c/main.nf#L995)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/4ff88ed06dbb90c656d681a10488520addebd47c/conf/base.config#L65) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/4ff88ed06dbb90c656d681a10488520addebd47c/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
