# Workflow outputs migration: raredisease

- Generated: 2026-07-01T00:47:02.553704+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:953`](https://github.com/nf-core/raredisease/blob/6fea9aea09786b85d38874766dc7b2243f31ea5c/main.nf#L953)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/6fea9aea09786b85d38874766dc7b2243f31ea5c/conf/base.config#L65) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/6fea9aea09786b85d38874766dc7b2243f31ea5c/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
