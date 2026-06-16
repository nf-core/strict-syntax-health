# Workflow outputs migration: rnafusion

- Generated: 2026-06-16T20:38:10.201583+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 35 `publishDir` references across 4 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L15) — 32 references
- [`modules/nf-core/umitools/extract/tests/nextflow.config`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/modules/nf-core/umitools/extract/tests/nextflow.config#L3) — 1 reference
- [`subworkflows/nf-core/fastq_align_star/tests/nextflow.config`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/subworkflows/nf-core/fastq_align_star/tests/nextflow.config#L3) — 1 reference
- [`subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config#L3) — 1 reference
