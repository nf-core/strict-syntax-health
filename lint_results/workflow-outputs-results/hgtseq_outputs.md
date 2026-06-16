# Workflow outputs migration: hgtseq

- Generated: 2026-06-16T19:28:03.411396+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 50 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L15) — 25 references
- [`tests/nextflow.config`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L16) — 25 references
