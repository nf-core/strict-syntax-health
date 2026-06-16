# Workflow outputs migration: slamseq

- Generated: 2026-06-16T19:43:57.372636+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 8 `publishDir` references across 1 file that should be migrated to the workflow `output {}` block:

- [`main.nf`](https://github.com/nf-core/slamseq/blob/c21d0faee30707ffe134f77e0b37887a1610503f/main.nf#L286) — 8 references
