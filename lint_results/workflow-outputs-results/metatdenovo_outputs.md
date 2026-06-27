# Workflow outputs migration: metatdenovo

- Generated: 2026-06-27T00:41:48.423036+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 14 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/metatdenovo/blob/afc7f125e115ae598add3b5494b1f40fd269bbe8/conf/modules.config#L13) — 13 references
- [`modules/nf-core/subread/featurecounts/tests/nextflow.config`](https://github.com/nf-core/metatdenovo/blob/afc7f125e115ae598add3b5494b1f40fd269bbe8/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3) — 1 reference
