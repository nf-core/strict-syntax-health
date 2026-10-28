# Workflow outputs migration: viralmetagenome

- Generated: 2026-10-28T00:20:42.583560+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 118 `publishDir` references across 4 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/viralmetagenome/blob/9b3ed25e48e256e5a660609aa36a7c3174cfe736/conf/modules.config#L15) — 115 references
- [`modules/nf-core/mmseqs/cluster/tests/nextflow.config`](https://github.com/nf-core/viralmetagenome/blob/9b3ed25e48e256e5a660609aa36a7c3174cfe736/modules/nf-core/mmseqs/cluster/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/mmseqs/linclust/tests/nextflow.config`](https://github.com/nf-core/viralmetagenome/blob/9b3ed25e48e256e5a660609aa36a7c3174cfe736/modules/nf-core/mmseqs/linclust/tests/nextflow.config#L3) — 1 reference
- [`subworkflows/local/map_reads/tests/nextflow.config`](https://github.com/nf-core/viralmetagenome/blob/9b3ed25e48e256e5a660609aa36a7c3174cfe736/subworkflows/local/map_reads/tests/nextflow.config#L21) — 1 reference
