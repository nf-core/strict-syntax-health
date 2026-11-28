# Workflow outputs migration: stampseq

- Generated: 2026-11-28T00:14:52.983638+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 26 `publishDir` references across 23 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/stampseq/blob/2a26d490a1aeafa6c4f3eed5f75a4f6ef4c34ea2/conf/modules.config#L13) — 3 references
- [`modules/local/metaplotr_sailor/main.nf`](https://github.com/nf-core/stampseq/blob/2a26d490a1aeafa6c4f3eed5f75a4f6ef4c34ea2/modules/local/metaplotr_sailor/main.nf#L7) — 2 references
- [`modules/local/cellranger/main.nf`](https://github.com/nf-core/stampseq/blob/2a26d490a1aeafa6c4f3eed5f75a4f6ef4c34ea2/modules/local/cellranger/main.nf#L13) — 1 reference
- [`modules/local/fastp/main.nf`](https://github.com/nf-core/stampseq/blob/2a26d490a1aeafa6c4f3eed5f75a4f6ef4c34ea2/modules/local/fastp/main.nf#L4) — 1 reference
- [`modules/local/featurecounts/main.nf`](https://github.com/nf-core/stampseq/blob/2a26d490a1aeafa6c4f3eed5f75a4f6ef4c34ea2/modules/local/featurecounts/main.nf#L9) — 1 reference
- [`modules/local/filter_edits_bulk/main.nf`](https://github.com/nf-core/stampseq/blob/2a26d490a1aeafa6c4f3eed5f75a4f6ef4c34ea2/modules/local/filter_edits_bulk/main.nf#L7) — 1 reference
- [`modules/local/filter_edits_sc/main.nf`](https://github.com/nf-core/stampseq/blob/2a26d490a1aeafa6c4f3eed5f75a4f6ef4c34ea2/modules/local/filter_edits_sc/main.nf#L7) — 1 reference
- [`modules/local/filter_site_frac_sc/main.nf`](https://github.com/nf-core/stampseq/blob/2a26d490a1aeafa6c4f3eed5f75a4f6ef4c34ea2/modules/local/filter_site_frac_sc/main.nf#L8) — 1 reference
- [`modules/local/flare/main.nf`](https://github.com/nf-core/stampseq/blob/2a26d490a1aeafa6c4f3eed5f75a4f6ef4c34ea2/modules/local/flare/main.nf#L22) — 1 reference
- [`modules/local/flare_generate_regions/main.nf`](https://github.com/nf-core/stampseq/blob/2a26d490a1aeafa6c4f3eed5f75a4f6ef4c34ea2/modules/local/flare_generate_regions/main.nf#L12) — 1 reference
- [`modules/local/infer_strandedness/main.nf`](https://github.com/nf-core/stampseq/blob/2a26d490a1aeafa6c4f3eed5f75a4f6ef4c34ea2/modules/local/infer_strandedness/main.nf#L7) — 1 reference
- [`modules/local/marine_bulk/main.nf`](https://github.com/nf-core/stampseq/blob/2a26d490a1aeafa6c4f3eed5f75a4f6ef4c34ea2/modules/local/marine_bulk/main.nf#L18) — 1 reference
- [`modules/local/marine_sc/main.nf`](https://github.com/nf-core/stampseq/blob/2a26d490a1aeafa6c4f3eed5f75a4f6ef4c34ea2/modules/local/marine_sc/main.nf#L14) — 1 reference
- [`modules/local/merge_counts/main.nf`](https://github.com/nf-core/stampseq/blob/2a26d490a1aeafa6c4f3eed5f75a4f6ef4c34ea2/modules/local/merge_counts/main.nf#L5) — 1 reference
- [`modules/local/merge_normalized_bulk/main.nf`](https://github.com/nf-core/stampseq/blob/2a26d490a1aeafa6c4f3eed5f75a4f6ef4c34ea2/modules/local/merge_normalized_bulk/main.nf#L6) — 1 reference
- [`modules/local/merge_normalized_sailor/main.nf`](https://github.com/nf-core/stampseq/blob/2a26d490a1aeafa6c4f3eed5f75a4f6ef4c34ea2/modules/local/merge_normalized_sailor/main.nf#L11) — 1 reference
- [`modules/local/metaplotr_bulk/main.nf`](https://github.com/nf-core/stampseq/blob/2a26d490a1aeafa6c4f3eed5f75a4f6ef4c34ea2/modules/local/metaplotr_bulk/main.nf#L7) — 1 reference
- [`modules/local/normalize_edits_bulk/main.nf`](https://github.com/nf-core/stampseq/blob/2a26d490a1aeafa6c4f3eed5f75a4f6ef4c34ea2/modules/local/normalize_edits_bulk/main.nf#L7) — 1 reference
- [`modules/local/normalize_edits_sailor/main.nf`](https://github.com/nf-core/stampseq/blob/2a26d490a1aeafa6c4f3eed5f75a4f6ef4c34ea2/modules/local/normalize_edits_sailor/main.nf#L7) — 1 reference
- [`modules/local/normalize_edits_sc/main.nf`](https://github.com/nf-core/stampseq/blob/2a26d490a1aeafa6c4f3eed5f75a4f6ef4c34ea2/modules/local/normalize_edits_sc/main.nf#L8) — 1 reference
- [`modules/local/sailor/main.nf`](https://github.com/nf-core/stampseq/blob/2a26d490a1aeafa6c4f3eed5f75a4f6ef4c34ea2/modules/local/sailor/main.nf#L8) — 1 reference
- [`modules/local/site_depth_sc/main.nf`](https://github.com/nf-core/stampseq/blob/2a26d490a1aeafa6c4f3eed5f75a4f6ef4c34ea2/modules/local/site_depth_sc/main.nf#L16) — 1 reference
- [`modules/local/star_align/main.nf`](https://github.com/nf-core/stampseq/blob/2a26d490a1aeafa6c4f3eed5f75a4f6ef4c34ea2/modules/local/star_align/main.nf#L4) — 1 reference
