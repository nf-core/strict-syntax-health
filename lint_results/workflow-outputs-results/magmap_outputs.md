# Workflow outputs migration: magmap

- Generated: 2026-09-16T00:20:43.261206+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 26 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/magmap/blob/c74cc6f8b826587e74b068fc40d4ee60897e7114/conf/modules.config#L15) — 25 references
- [`modules/nf-core/subread/featurecounts/tests/nextflow.config`](https://github.com/nf-core/magmap/blob/c74cc6f8b826587e74b068fc40d4ee60897e7114/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3) — 1 reference
