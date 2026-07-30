# Workflow outputs migration: proteinfold

- Generated: 2026-07-30T00:30:36.050964+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 51 `publishDir` references across 10 files that should be migrated to the workflow `output {}` block:

- [`conf/modules_helixfold3.config`](https://github.com/nf-core/proteinfold/blob/7d7a5ed134cc23afa6b90ae034b5a6f19d6bf7c0/conf/modules_helixfold3.config#L20) — 13 references
- [`conf/modules_alphafold2.config`](https://github.com/nf-core/proteinfold/blob/7d7a5ed134cc23afa6b90ae034b5a6f19d6bf7c0/conf/modules_alphafold2.config#L19) — 10 references
- [`conf/modules_boltz.config`](https://github.com/nf-core/proteinfold/blob/7d7a5ed134cc23afa6b90ae034b5a6f19d6bf7c0/conf/modules_boltz.config#L18) — 7 references
- [`conf/modules.config`](https://github.com/nf-core/proteinfold/blob/7d7a5ed134cc23afa6b90ae034b5a6f19d6bf7c0/conf/modules.config#L18) — 6 references
- [`conf/modules_alphafold3.config`](https://github.com/nf-core/proteinfold/blob/7d7a5ed134cc23afa6b90ae034b5a6f19d6bf7c0/conf/modules_alphafold3.config#L19) — 5 references
- [`conf/modules_rosettafold2na.config`](https://github.com/nf-core/proteinfold/blob/7d7a5ed134cc23afa6b90ae034b5a6f19d6bf7c0/conf/modules_rosettafold2na.config#L25) — 3 references
- [`conf/modules_colabfold.config`](https://github.com/nf-core/proteinfold/blob/7d7a5ed134cc23afa6b90ae034b5a6f19d6bf7c0/conf/modules_colabfold.config#L17) — 2 references
- [`conf/modules_esmfold.config`](https://github.com/nf-core/proteinfold/blob/7d7a5ed134cc23afa6b90ae034b5a6f19d6bf7c0/conf/modules_esmfold.config#L16) — 2 references
- [`conf/modules_rosettafold_all_atom.config`](https://github.com/nf-core/proteinfold/blob/7d7a5ed134cc23afa6b90ae034b5a6f19d6bf7c0/conf/modules_rosettafold_all_atom.config#L15) — 2 references
- [`modules/nf-core/mmseqs/createindex/tests/nextflow.config`](https://github.com/nf-core/proteinfold/blob/7d7a5ed134cc23afa6b90ae034b5a6f19d6bf7c0/modules/nf-core/mmseqs/createindex/tests/nextflow.config#L3) — 1 reference
