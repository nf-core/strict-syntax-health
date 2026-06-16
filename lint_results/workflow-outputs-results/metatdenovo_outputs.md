# Workflow outputs migration: metatdenovo

- Generated: 2026-06-16T19:31:11.114506+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 14 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L13) — 13 references
- [`modules/nf-core/subread/featurecounts/tests/nextflow.config`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3) — 1 reference
