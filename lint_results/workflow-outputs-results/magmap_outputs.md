# Workflow outputs migration: magmap

- Generated: 2026-11-18T00:13:19.745864+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 30 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/magmap/blob/c73df7093dbd8c69bd0b639c67ed8471ed138a3c/conf/modules.config#L15) — 29 references
- [`modules/nf-core/subread/featurecounts/tests/nextflow.config`](https://github.com/nf-core/magmap/blob/c73df7093dbd8c69bd0b639c67ed8471ed138a3c/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3) — 1 reference
