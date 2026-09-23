# Workflow outputs migration: smrnaseq

- Generated: 2026-09-23T00:26:20.528055+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 53 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/smrnaseq/blob/8dea8e1b8e5a4955230b55867a663a034b13e9c2/conf/modules.config#L20) — 52 references
- [`modules/nf-core/umitools/extract/tests/nextflow.config`](https://github.com/nf-core/smrnaseq/blob/8dea8e1b8e5a4955230b55867a663a034b13e9c2/modules/nf-core/umitools/extract/tests/nextflow.config#L3) — 1 reference
