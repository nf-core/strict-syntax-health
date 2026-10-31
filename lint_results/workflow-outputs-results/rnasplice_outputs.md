# Workflow outputs migration: rnasplice

- Generated: 2026-10-31T00:16:47.557649+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 81 `publishDir` references across 6 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/rnasplice/blob/0f433570768f871ab973daaca939e8e651dc42e6/conf/modules.config#L16) — 76 references
- [`modules/nf-core/rseqc/inferexperiment/tests/nextflow.config`](https://github.com/nf-core/rnasplice/blob/0f433570768f871ab973daaca939e8e651dc42e6/modules/nf-core/rseqc/inferexperiment/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/subread/featurecounts/tests/nextflow.config`](https://github.com/nf-core/rnasplice/blob/0f433570768f871ab973daaca939e8e651dc42e6/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/umitools/extract/tests/nextflow.config`](https://github.com/nf-core/rnasplice/blob/0f433570768f871ab973daaca939e8e651dc42e6/modules/nf-core/umitools/extract/tests/nextflow.config#L3) — 1 reference
- [`subworkflows/nf-core/bedgraph_bedclip_bedgraphtobigwig/tests/nextflow.config`](https://github.com/nf-core/rnasplice/blob/0f433570768f871ab973daaca939e8e651dc42e6/subworkflows/nf-core/bedgraph_bedclip_bedgraphtobigwig/tests/nextflow.config#L3) — 1 reference
- [`subworkflows/nf-core/fastq_subsample_fq_salmon/tests/nextflow.config`](https://github.com/nf-core/rnasplice/blob/0f433570768f871ab973daaca939e8e651dc42e6/subworkflows/nf-core/fastq_subsample_fq_salmon/tests/nextflow.config#L3) — 1 reference
