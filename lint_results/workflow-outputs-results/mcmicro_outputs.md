# Workflow outputs migration: mcmicro

- Generated: 2026-10-06T00:21:56.044357+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 10 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/mcmicro/blob/c3d46693e94b7e2645bee564f08a73fdeaeefb32/conf/modules.config#L15) — 9 references
- [`tests/lib/utils.nf`](https://github.com/nf-core/mcmicro/blob/c3d46693e94b7e2645bee564f08a73fdeaeefb32/tests/lib/utils.nf#L9) — 1 reference
