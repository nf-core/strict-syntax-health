# Workflow outputs migration: rarevariantburden

- Generated: 2026-07-28T00:33:24.614814+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 17 `publishDir` references across 1 file that should be migrated to the workflow `output {}` block:

- [`modules/local/cocorv/main.nf`](https://github.com/nf-core/rarevariantburden/blob/8810e3d0f3927a3995a59221bad0b3eea15395a9/modules/local/cocorv/main.nf#L52) — 17 references
