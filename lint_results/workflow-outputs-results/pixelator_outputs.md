# Workflow outputs migration: pixelator

- Generated: 2026-07-23T00:32:02.494258+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 12 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.pna.config`](https://github.com/nf-core/pixelator/blob/53d856c06c51dd8fb4983b197ed9d57ba6b985e5/conf/modules.pna.config#L30) — 8 references
- [`conf/modules.config`](https://github.com/nf-core/pixelator/blob/53d856c06c51dd8fb4983b197ed9d57ba6b985e5/conf/modules.config#L16) — 4 references
