# Workflow outputs migration: ribomsqc

- Generated: 2026-11-19T00:15:15.040208+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 1 `publishDir` reference across 1 file that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/ribomsqc/blob/6d0fcedd95f444ce8b405d46d0677a7ff277e594/conf/modules.config#L15) — 1 reference
