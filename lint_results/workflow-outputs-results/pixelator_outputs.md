# Workflow outputs migration: pixelator

- Generated: 2026-06-23T00:43:22.656800+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 12 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.pna.config`](https://github.com/nf-core/pixelator/blob/a2470e2c5fd51970ca5735fe0ce8d03a1c80c4e3/conf/modules.pna.config#L30) — 8 references
- [`conf/modules.config`](https://github.com/nf-core/pixelator/blob/a2470e2c5fd51970ca5735fe0ce8d03a1c80c4e3/conf/modules.config#L16) — 4 references
