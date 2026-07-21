# Workflow outputs migration: differentialabundance

- Generated: 2026-07-21T00:29:27.916093+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:275`](https://github.com/nf-core/differentialabundance/blob/0dca5f186f7b325f23b72c5dc458d48883875a20/main.nf#L275)

## Legacy `publishDir` references

Found 10 `publishDir` references across 5 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/differentialabundance/blob/0dca5f186f7b325f23b72c5dc458d48883875a20/conf/modules.config#L257) — 2 references
- [`modules/nf-core/limma/differential/tests/nextflow.config`](https://github.com/nf-core/differentialabundance/blob/0dca5f186f7b325f23b72c5dc458d48883875a20/modules/nf-core/limma/differential/tests/nextflow.config#L12) — 2 references
- [`modules/nf-core/limma/differential/tests/nextflow.exclude_samples.config`](https://github.com/nf-core/differentialabundance/blob/0dca5f186f7b325f23b72c5dc458d48883875a20/modules/nf-core/limma/differential/tests/nextflow.exclude_samples.config#L13) — 2 references
- [`modules/nf-core/limma/differential/tests/nextflow.subset_to_contrast.config`](https://github.com/nf-core/differentialabundance/blob/0dca5f186f7b325f23b72c5dc458d48883875a20/modules/nf-core/limma/differential/tests/nextflow.subset_to_contrast.config#L12) — 2 references
- [`subworkflows/nf-core/abundance_differential_filter/tests/limma_basic_microarray.config`](https://github.com/nf-core/differentialabundance/blob/0dca5f186f7b325f23b72c5dc458d48883875a20/subworkflows/nf-core/abundance_differential_filter/tests/limma_basic_microarray.config#L18) — 2 references
