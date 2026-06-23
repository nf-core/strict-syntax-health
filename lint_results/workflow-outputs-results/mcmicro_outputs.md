# Workflow outputs migration: mcmicro

- Generated: 2026-06-23T00:42:30.519657+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 10 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/mcmicro/blob/4fa1c1f1866b9c427e40a04326b56969c117bae4/conf/modules.config#L15) — 9 references
- [`tests/lib/utils.nf`](https://github.com/nf-core/mcmicro/blob/4fa1c1f1866b9c427e40a04326b56969c117bae4/tests/lib/utils.nf#L15) — 1 reference
