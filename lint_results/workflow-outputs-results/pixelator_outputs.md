# Workflow outputs migration: pixelator

- Generated: 2026-11-17T00:15:35.790341+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 10 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.pna.config`](https://github.com/nf-core/pixelator/blob/b8a700890ad7cae34df6fb2ed1578f838bda5f83/conf/modules.pna.config#L26) — 7 references
- [`conf/modules.config`](https://github.com/nf-core/pixelator/blob/b8a700890ad7cae34df6fb2ed1578f838bda5f83/conf/modules.config#L16) — 3 references
