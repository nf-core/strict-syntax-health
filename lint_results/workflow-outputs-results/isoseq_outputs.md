# Workflow outputs migration: isoseq

- Generated: 2026-09-22T00:21:50.117875+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 15 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/isoseq/blob/aacae9d598e4c9ae57729a6c0dec6a27be640d25/conf/modules.config#L15) — 14 references
- [`modules/nf-core/lima/tests/nextflow.config`](https://github.com/nf-core/isoseq/blob/aacae9d598e4c9ae57729a6c0dec6a27be640d25/modules/nf-core/lima/tests/nextflow.config#L3) — 1 reference
