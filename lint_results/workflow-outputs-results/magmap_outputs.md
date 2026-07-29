# Workflow outputs migration: magmap

- Generated: 2026-07-29T00:28:46.363669+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 25 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/magmap/blob/d6618ac43fc4e571b3eaa346b101773d118c5f94/conf/modules.config#L15) — 24 references
- [`modules/nf-core/subread/featurecounts/tests/nextflow.config`](https://github.com/nf-core/magmap/blob/d6618ac43fc4e571b3eaa346b101773d118c5f94/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3) — 1 reference
