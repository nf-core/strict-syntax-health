# Workflow outputs migration: mag

- Generated: 2026-08-13T00:21:23.524199+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 41 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/mag/blob/2f3655c78b0e5ec7373df35971e8d92bc6c46333/conf/modules.config#L16) — 40 references
- [`modules/nf-core/dastool/dastool/tests/nextflow.config`](https://github.com/nf-core/mag/blob/2f3655c78b0e5ec7373df35971e8d92bc6c46333/modules/nf-core/dastool/dastool/tests/nextflow.config#L3) — 1 reference
