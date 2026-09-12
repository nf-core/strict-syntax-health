# Workflow outputs migration: metatdenovo

- Generated: 2026-09-12T00:21:35.764018+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 17 `publishDir` references across 4 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/metatdenovo/blob/c0d4f79421c4ac1cf9671bcb3340dc4de59d13db/conf/modules.config#L13) — 14 references
- [`modules/nf-core/mmseqs/cluster/tests/nextflow.config`](https://github.com/nf-core/metatdenovo/blob/c0d4f79421c4ac1cf9671bcb3340dc4de59d13db/modules/nf-core/mmseqs/cluster/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/mmseqs/linclust/tests/nextflow.config`](https://github.com/nf-core/metatdenovo/blob/c0d4f79421c4ac1cf9671bcb3340dc4de59d13db/modules/nf-core/mmseqs/linclust/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/subread/featurecounts/tests/nextflow.config`](https://github.com/nf-core/metatdenovo/blob/c0d4f79421c4ac1cf9671bcb3340dc4de59d13db/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3) — 1 reference
