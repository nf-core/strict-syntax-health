# Workflow outputs migration: rarevariantburden

- Generated: 2026-07-30T00:31:28.974400+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 17 `publishDir` references across 1 file that should be migrated to the workflow `output {}` block:

- [`modules/local/cocorv/main.nf`](https://github.com/nf-core/rarevariantburden/blob/d1e22b021c93e69c3f39e1be56288394edcf22bc/modules/local/cocorv/main.nf#L52) — 17 references
