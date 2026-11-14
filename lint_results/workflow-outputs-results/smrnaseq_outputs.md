# Workflow outputs migration: smrnaseq

- Generated: 2026-11-14T00:15:08.441634+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:166`](https://github.com/nf-core/smrnaseq/blob/7ca21c32984d1cec67b59db5b8b088893dbf6045/main.nf#L166)

## Legacy `publishDir` references

Found 1 `publishDir` reference across 1 file that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/smrnaseq/blob/7ca21c32984d1cec67b59db5b8b088893dbf6045/conf/modules.config#L198) — 1 reference
