# Workflow outputs migration: rarevariantburden

- Generated: 2026-06-16T19:38:33.213071+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 17 `publishDir` references across 1 file that should be migrated to the workflow `output {}` block:

- [`modules/local/cocorv/main.nf`](https://github.com/nf-core/rarevariantburden/blob/e9392c4294ecdd4f6f984b9c235eb220306455be/modules/local/cocorv/main.nf#L28) — 17 references
