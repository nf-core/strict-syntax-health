# Workflow outputs migration: smrnaseq

- Generated: 2026-10-30T00:21:01.534296+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 53 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/smrnaseq/blob/2c2793ac05b4f9ab0cb5ab8141b7baa0594ab0c9/conf/modules.config#L20) — 52 references
- [`modules/nf-core/umitools/extract/tests/nextflow.config`](https://github.com/nf-core/smrnaseq/blob/2c2793ac05b4f9ab0cb5ab8141b7baa0594ab0c9/modules/nf-core/umitools/extract/tests/nextflow.config#L3) — 1 reference
