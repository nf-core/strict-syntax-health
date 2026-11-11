# Workflow outputs migration: smrnaseq

- Generated: 2026-11-11T00:19:16.059770+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 53 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/smrnaseq/blob/559916f75f1f39a11b577505ef069ba724f2727b/conf/modules.config#L20) — 52 references
- [`modules/nf-core/umitools/extract/tests/nextflow.config`](https://github.com/nf-core/smrnaseq/blob/559916f75f1f39a11b577505ef069ba724f2727b/modules/nf-core/umitools/extract/tests/nextflow.config#L3) — 1 reference
