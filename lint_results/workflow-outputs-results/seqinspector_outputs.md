# Workflow outputs migration: seqinspector

- Generated: 2026-06-16T18:07:52.647313+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:128`](https://github.com/nf-core/seqinspector/blob/3f446363fc41b4a503885154373da0982a6d11dd/main.nf#L128)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`nextflow.config`](https://github.com/nf-core/seqinspector/blob/3f446363fc41b4a503885154373da0982a6d11dd/nextflow.config#L80) — 1 reference
- [`workflows/seqinspector.nf`](https://github.com/nf-core/seqinspector/blob/3f446363fc41b4a503885154373da0982a6d11dd/workflows/seqinspector.nf#L102) — 1 reference
