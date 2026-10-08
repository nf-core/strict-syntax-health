# Workflow outputs migration: metatdenovo

- Generated: 2026-10-08T00:26:50.511399+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 18 `publishDir` references across 4 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/metatdenovo/blob/36c67a0d65ff985622b0391d694d6ce8533092c4/conf/modules.config#L13) — 15 references
- [`modules/nf-core/mmseqs/cluster/tests/nextflow.config`](https://github.com/nf-core/metatdenovo/blob/36c67a0d65ff985622b0391d694d6ce8533092c4/modules/nf-core/mmseqs/cluster/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/mmseqs/linclust/tests/nextflow.config`](https://github.com/nf-core/metatdenovo/blob/36c67a0d65ff985622b0391d694d6ce8533092c4/modules/nf-core/mmseqs/linclust/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/subread/featurecounts/tests/nextflow.config`](https://github.com/nf-core/metatdenovo/blob/36c67a0d65ff985622b0391d694d6ce8533092c4/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3) — 1 reference
