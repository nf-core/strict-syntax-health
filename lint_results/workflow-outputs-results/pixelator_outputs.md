# Workflow outputs migration: pixelator

- Generated: 2026-08-18T00:14:09.932116+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 12 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.pna.config`](https://github.com/nf-core/pixelator/blob/6419699ab22766a37a73bb8f78bfc67b80939a04/conf/modules.pna.config#L30) — 8 references
- [`conf/modules.config`](https://github.com/nf-core/pixelator/blob/6419699ab22766a37a73bb8f78bfc67b80939a04/conf/modules.config#L16) — 4 references
