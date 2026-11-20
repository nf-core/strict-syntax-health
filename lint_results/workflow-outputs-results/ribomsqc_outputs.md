# Workflow outputs migration: ribomsqc

- Generated: 2026-11-20T00:13:49.610782+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 1 `publishDir` reference across 1 file that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/ribomsqc/blob/92cb1ebcfa391eda417ed1ef9f8bb8571d230345/conf/modules.config#L15) — 1 reference
