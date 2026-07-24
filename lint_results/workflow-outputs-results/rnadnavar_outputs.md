# Workflow outputs migration: rnadnavar

- Generated: 2026-07-24T00:28:19.966795+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 98 `publishDir` references across 28 files that should be migrated to the workflow `output {}` block:

- [`conf/modules/quality_control/quality_control.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/conf/modules/quality_control/quality_control.config#L20) — 12 references
- [`conf/modules/prepare_resources/prepare_genome.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/conf/modules/prepare_resources/prepare_genome.config#L20) — 11 references
- [`conf/modules/alignment/bam_align.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/conf/modules/alignment/bam_align.config#L35) — 10 references
- [`conf/modules/alignment/alignment_to_fastq.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/conf/modules/alignment/alignment_to_fastq.config#L21) — 8 references
- [`conf/modules/variant_calling/mutect2.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/conf/modules/variant_calling/mutect2.config#L25) — 8 references
- [`conf/modules/prepare_resources/prepare_intervals.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/conf/modules/prepare_resources/prepare_intervals.config#L19) — 6 references
- [`conf/modules/gatk4_preprocessing/markduplicates.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/conf/modules/gatk4_preprocessing/markduplicates.config#L28) — 5 references
- [`conf/modules/gatk4_preprocessing/splitncigarreads.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/conf/modules/gatk4_preprocessing/splitncigarreads.config#L21) — 5 references
- [`conf/modules/gatk4_preprocessing/recalibrate.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/conf/modules/gatk4_preprocessing/recalibrate.config#L20) — 4 references
- [`conf/modules/consensus/vcf_consensus.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/conf/modules/consensus/vcf_consensus.config#L20) — 3 references
- [`conf/modules/variant_calling/sage.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/conf/modules/variant_calling/sage.config#L27) — 3 references
- [`conf/modules/annotate/annotate.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/conf/modules/annotate/annotate.config#L31) — 2 references
- [`conf/modules/filtering/maf_filtering.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/conf/modules/filtering/maf_filtering.config#L25) — 2 references
- [`conf/modules/gatk4_preprocessing/prepare_recalibration.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/conf/modules/gatk4_preprocessing/prepare_recalibration.config#L21) — 2 references
- [`conf/modules/normalize/vt.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/conf/modules/normalize/vt.config#L21) — 2 references
- [`conf/modules/prepare_realignment/extract_reads_id.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/conf/modules/prepare_realignment/extract_reads_id.config#L21) — 2 references
- [`conf/modules/variant_calling/strelka.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/conf/modules/variant_calling/strelka.config#L23) — 2 references
- [`conf/modules.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/conf/modules.config#L15) — 1 reference
- [`conf/modules/modules.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/conf/modules/modules.config#L15) — 1 reference
- [`conf/modules/prepare_realignment/filtersamreads.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/conf/modules/prepare_realignment/filtersamreads.config#L21) — 1 reference
- [`conf/modules/prepare_resources/prepare_cache.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/conf/modules/prepare_resources/prepare_cache.config#L22) — 1 reference
- [`conf/modules/quality_control/trimming.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/conf/modules/quality_control/trimming.config#L28) — 1 reference
- [`conf/modules/variant_calling/mutect2_joint.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/conf/modules/variant_calling/mutect2_joint.config#L19) — 1 reference
- [`conf/modules/variant_calling/variant_calling.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/conf/modules/variant_calling/variant_calling.config#L20) — 1 reference
- [`modules/nf-core/gatk4/variantrecalibrator/tests/AS.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/modules/nf-core/gatk4/variantrecalibrator/tests/AS.config#L3) — 1 reference
- [`modules/nf-core/gatk4/variantrecalibrator/tests/noAS.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/modules/nf-core/gatk4/variantrecalibrator/tests/noAS.config#L3) — 1 reference
- [`subworkflows/nf-core/fastq_align_star/tests/nextflow.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/subworkflows/nf-core/fastq_align_star/tests/nextflow.config#L3) — 1 reference
- [`subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config`](https://github.com/nf-core/rnadnavar/blob/3279bf473055f67ed359b8ba95463d86456bea1d/subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config#L3) — 1 reference
