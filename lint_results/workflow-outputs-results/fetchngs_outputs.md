# Workflow outputs migration: fetchngs

- Generated: 2026-08-11T00:15:18.327139+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 10 `publishDir` references across 10 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/fetchngs/blob/536465a126754078a8328fc67eacefd79a57b0f2/conf/base.config#L16) — 1 reference
- [`modules/local/aspera_cli/nextflow.config`](https://github.com/nf-core/fetchngs/blob/536465a126754078a8328fc67eacefd79a57b0f2/modules/local/aspera_cli/nextflow.config#L4) — 1 reference
- [`modules/local/multiqc_mappings_config/nextflow.config`](https://github.com/nf-core/fetchngs/blob/536465a126754078a8328fc67eacefd79a57b0f2/modules/local/multiqc_mappings_config/nextflow.config#L3) — 1 reference
- [`modules/local/sra_fastq_ftp/nextflow.config`](https://github.com/nf-core/fetchngs/blob/536465a126754078a8328fc67eacefd79a57b0f2/modules/local/sra_fastq_ftp/nextflow.config#L4) — 1 reference
- [`modules/local/sra_ids_to_runinfo/nextflow.config`](https://github.com/nf-core/fetchngs/blob/536465a126754078a8328fc67eacefd79a57b0f2/modules/local/sra_ids_to_runinfo/nextflow.config#L3) — 1 reference
- [`modules/local/sra_runinfo_to_ftp/nextflow.config`](https://github.com/nf-core/fetchngs/blob/536465a126754078a8328fc67eacefd79a57b0f2/modules/local/sra_runinfo_to_ftp/nextflow.config#L3) — 1 reference
- [`modules/local/sra_to_samplesheet/nextflow.config`](https://github.com/nf-core/fetchngs/blob/536465a126754078a8328fc67eacefd79a57b0f2/modules/local/sra_to_samplesheet/nextflow.config#L3) — 1 reference
- [`modules/nf-core/fastqdl/nextflow.config`](https://github.com/nf-core/fetchngs/blob/536465a126754078a8328fc67eacefd79a57b0f2/modules/nf-core/fastqdl/nextflow.config#L3) — 1 reference
- [`modules/nf-core/sratools/fasterqdump/nextflow.config`](https://github.com/nf-core/fetchngs/blob/536465a126754078a8328fc67eacefd79a57b0f2/modules/nf-core/sratools/fasterqdump/nextflow.config#L4) — 1 reference
- [`modules/nf-core/sratools/prefetch/nextflow.config`](https://github.com/nf-core/fetchngs/blob/536465a126754078a8328fc67eacefd79a57b0f2/modules/nf-core/sratools/prefetch/nextflow.config#L3) — 1 reference
