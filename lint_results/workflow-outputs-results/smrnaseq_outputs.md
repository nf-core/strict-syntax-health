# Workflow outputs migration: smrnaseq

- Generated: 2026-09-24T00:22:03.121195+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 53 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/smrnaseq/blob/b8bf7d26d544b438549bd261510e112486126cad/conf/modules.config#L20) — 52 references
- [`modules/nf-core/umitools/extract/tests/nextflow.config`](https://github.com/nf-core/smrnaseq/blob/b8bf7d26d544b438549bd261510e112486126cad/modules/nf-core/umitools/extract/tests/nextflow.config#L3) — 1 reference
