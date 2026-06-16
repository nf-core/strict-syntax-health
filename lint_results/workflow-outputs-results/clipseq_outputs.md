# Workflow outputs migration: clipseq

- Generated: 2026-06-16T20:19:18.006854+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 24 `publishDir` references across 1 file that should be migrated to the workflow `output {}` block:

- [`main.nf`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L247) — 24 references
