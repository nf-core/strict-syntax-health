# Workflow outputs migration: raredisease

- Generated: 2026-11-12T00:17:28.856968+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:1036`](https://github.com/nf-core/raredisease/blob/659334927edb30eb88da8a04f5ece8b37537627c/main.nf#L1036)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/659334927edb30eb88da8a04f5ece8b37537627c/conf/base.config#L67) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/659334927edb30eb88da8a04f5ece8b37537627c/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
