# Workflow outputs migration: hic

- Generated: 2026-11-28T00:12:27.327111+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 45 `publishDir` references across 1 file that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/hic/blob/b98ef122a5c4dc4e1c25daf67255a956bc57d0c8/conf/modules.config#L3) — 45 references
