# Workflow outputs migration: metatdenovo

- Generated: 2026-10-24T00:20:45.012243+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 18 `publishDir` references across 4 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/metatdenovo/blob/017514c173874c76b8841d38ff1c54dbeb6e2eed/conf/modules.config#L13) — 15 references
- [`modules/nf-core/mmseqs/cluster/tests/nextflow.config`](https://github.com/nf-core/metatdenovo/blob/017514c173874c76b8841d38ff1c54dbeb6e2eed/modules/nf-core/mmseqs/cluster/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/mmseqs/linclust/tests/nextflow.config`](https://github.com/nf-core/metatdenovo/blob/017514c173874c76b8841d38ff1c54dbeb6e2eed/modules/nf-core/mmseqs/linclust/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/subread/featurecounts/tests/nextflow.config`](https://github.com/nf-core/metatdenovo/blob/017514c173874c76b8841d38ff1c54dbeb6e2eed/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3) — 1 reference
