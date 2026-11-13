# Workflow outputs migration: proteinfamilies

- Generated: 2026-11-13T00:16:38.279564+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:181`](https://github.com/nf-core/proteinfamilies/blob/6645c6329868614bcf58b3ddad4526b2a152271e/main.nf#L181)

## Legacy `publishDir` references

Found 81 `publishDir` references across 3 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/proteinfamilies/blob/6645c6329868614bcf58b3ddad4526b2a152271e/conf/modules.config#L15) — 79 references
- [`modules/nf-core/mmseqs/cluster/tests/nextflow.config`](https://github.com/nf-core/proteinfamilies/blob/6645c6329868614bcf58b3ddad4526b2a152271e/modules/nf-core/mmseqs/cluster/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/mmseqs/linclust/tests/nextflow.config`](https://github.com/nf-core/proteinfamilies/blob/6645c6329868614bcf58b3ddad4526b2a152271e/modules/nf-core/mmseqs/linclust/tests/nextflow.config#L3) — 1 reference
