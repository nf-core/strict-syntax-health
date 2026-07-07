# Workflow outputs migration: viralmetagenome

- Generated: 2026-07-07T00:40:15.684343+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 116 `publishDir` references across 4 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/viralmetagenome/blob/bfd7357535c9bec31bfc64abd460480b4e26a8dc/conf/modules.config#L15) — 113 references
- [`modules/nf-core/mmseqs/cluster/tests/nextflow.config`](https://github.com/nf-core/viralmetagenome/blob/bfd7357535c9bec31bfc64abd460480b4e26a8dc/modules/nf-core/mmseqs/cluster/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/mmseqs/linclust/tests/nextflow.config`](https://github.com/nf-core/viralmetagenome/blob/bfd7357535c9bec31bfc64abd460480b4e26a8dc/modules/nf-core/mmseqs/linclust/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/umitools/extract/tests/nextflow.config`](https://github.com/nf-core/viralmetagenome/blob/bfd7357535c9bec31bfc64abd460480b4e26a8dc/modules/nf-core/umitools/extract/tests/nextflow.config#L3) — 1 reference
