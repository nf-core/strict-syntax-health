# Workflow outputs migration: hgtseq

- Generated: 2026-11-03T00:12:36.286033+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 50 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/hgtseq/blob/b076ea7adc3a80581a649dbd7d3e0ece53a66dcb/conf/modules.config#L15) — 25 references
- [`tests/nextflow.config`](https://github.com/nf-core/hgtseq/blob/b076ea7adc3a80581a649dbd7d3e0ece53a66dcb/tests/nextflow.config#L16) — 25 references
