# Workflow outputs migration: smrnaseq

- Generated: 2026-11-21T00:14:16.190208+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:247`](https://github.com/nf-core/smrnaseq/blob/861a631eb9c7669d04965feb9a12ce87b9bef99e/main.nf#L247)

## Legacy `publishDir` references

Found 1 `publishDir` reference across 1 file that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/smrnaseq/blob/861a631eb9c7669d04965feb9a12ce87b9bef99e/conf/modules.config#L198) — 1 reference
