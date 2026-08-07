# Workflow outputs migration: proteinfamilies

- Generated: 2026-08-07T01:15:32.628325+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:106`](https://github.com/nf-core/proteinfamilies/blob/9419af6af2067e303e9a64f9aa7f20b6a8c073b9/main.nf#L106)

## Legacy `publishDir` references

Found 79 `publishDir` references across 3 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/proteinfamilies/blob/9419af6af2067e303e9a64f9aa7f20b6a8c073b9/conf/modules.config#L15) — 77 references
- [`modules/nf-core/mmseqs/cluster/tests/nextflow.config`](https://github.com/nf-core/proteinfamilies/blob/9419af6af2067e303e9a64f9aa7f20b6a8c073b9/modules/nf-core/mmseqs/cluster/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/mmseqs/linclust/tests/nextflow.config`](https://github.com/nf-core/proteinfamilies/blob/9419af6af2067e303e9a64f9aa7f20b6a8c073b9/modules/nf-core/mmseqs/linclust/tests/nextflow.config#L3) — 1 reference
