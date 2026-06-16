# Workflow outputs migration: diaproteomics

- Generated: 2026-06-16T20:21:58.648978+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 13 `publishDir` references across 1 file that should be migrated to the workflow `output {}` block:

- [`main.nf`](https://github.com/nf-core/diaproteomics/blob/92314aba5cc590906a4e4616be55781a1dd4d530/main.nf#L323) — 13 references
