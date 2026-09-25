# Workflow outputs migration: rnasplice

- Generated: 2026-09-25T00:23:48.519607+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 73 `publishDir` references across 4 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/rnasplice/blob/1b447239488097651d8eac44bca2c1556865eb0f/conf/modules.config#L16) — 70 references
- [`modules/nf-core/subread/featurecounts/tests/nextflow.config`](https://github.com/nf-core/rnasplice/blob/1b447239488097651d8eac44bca2c1556865eb0f/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/umitools/extract/tests/nextflow.config`](https://github.com/nf-core/rnasplice/blob/1b447239488097651d8eac44bca2c1556865eb0f/modules/nf-core/umitools/extract/tests/nextflow.config#L3) — 1 reference
- [`subworkflows/nf-core/bedgraph_bedclip_bedgraphtobigwig/tests/nextflow.config`](https://github.com/nf-core/rnasplice/blob/1b447239488097651d8eac44bca2c1556865eb0f/subworkflows/nf-core/bedgraph_bedclip_bedgraphtobigwig/tests/nextflow.config#L3) — 1 reference
