# Workflow outputs migration: raredisease

- Generated: 2026-08-05T00:30:40.783819+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:1029`](https://github.com/nf-core/raredisease/blob/1be665303a37802bf0bfc0051f2eb236e08784e0/main.nf#L1029)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/1be665303a37802bf0bfc0051f2eb236e08784e0/conf/base.config#L65) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/1be665303a37802bf0bfc0051f2eb236e08784e0/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
