# Workflow outputs migration: mnaseseq

- Generated: 2026-06-16T19:32:20.528195+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 26 `publishDir` references across 1 file that should be migrated to the workflow `output {}` block:

- [`main.nf`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L279) — 26 references
