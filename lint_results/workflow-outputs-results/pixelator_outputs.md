# Workflow outputs migration: pixelator

- Generated: 2026-11-13T00:16:12.305889+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 10 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.pna.config`](https://github.com/nf-core/pixelator/blob/9479b2332c2a3e0f3173a372aa944740364d30bc/conf/modules.pna.config#L26) — 7 references
- [`conf/modules.config`](https://github.com/nf-core/pixelator/blob/9479b2332c2a3e0f3173a372aa944740364d30bc/conf/modules.config#L16) — 3 references
