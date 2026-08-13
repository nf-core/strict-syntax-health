# Workflow outputs migration: sarek

- Generated: 2026-08-13T00:23:42.268821+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:386`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/main.nf#L386)

## Legacy `publishDir` references

Found 191 `publishDir` references across 40 files that should be migrated to the workflow `output {}` block:

- [`conf/modules/varlociraptor.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/varlociraptor.config#L22) — 24 references
- [`conf/modules/prepare_genome.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/prepare_genome.config#L18) — 19 references
- [`conf/modules/post_variant_calling.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/post_variant_calling.config#L24) — 10 references
- [`conf/modules/alignment_to_fastq.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/alignment_to_fastq.config#L21) — 8 references
- [`conf/modules/joint_germline.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/joint_germline.config#L23) — 8 references
- [`conf/modules/modules.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/modules.config#L19) — 8 references
- [`conf/modules/mutect2.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/mutect2.config#L22) — 8 references
- [`conf/modules/umi.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/umi.config#L22) — 8 references
- [`conf/modules/annotate.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/annotate.config#L22) — 7 references
- [`conf/modules/sentieon_joint_germline.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/sentieon_joint_germline.config#L21) — 7 references
- [`conf/modules/freebayes.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/freebayes.config#L20) — 6 references
- [`conf/modules/markduplicates.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/markduplicates.config#L21) — 6 references
- [`conf/modules/controlfreec.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/controlfreec.config#L19) — 5 references
- [`conf/modules/haplotypecaller.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/haplotypecaller.config#L25) — 5 references
- [`conf/modules/recalibrate.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/recalibrate.config#L24) — 5 references
- [`conf/modules/aligner_parabricks.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/aligner_parabricks.config#L27) — 4 references
- [`conf/modules/cnvkit.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/cnvkit.config#L21) — 4 references
- [`conf/modules/mpileup.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/mpileup.config#L19) — 4 references
- [`conf/modules/sentieon_dnascope.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/sentieon_dnascope.config#L21) — 4 references
- [`conf/modules/sentieon_haplotyper.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/sentieon_haplotyper.config#L21) — 4 references
- [`conf/modules/muse.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/muse.config#L22) — 3 references
- [`conf/modules/prepare_intervals.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/prepare_intervals.config#L24) — 3 references
- [`conf/modules/tiddit.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/tiddit.config#L22) — 3 references
- [`conf/modules/aligner.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/aligner.config#L37) — 2 references
- [`conf/modules/deepvariant.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/deepvariant.config#L25) — 2 references
- [`conf/modules/download_cache.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/download_cache.config#L21) — 2 references
- [`conf/modules/indexcov.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/indexcov.config#L8) — 2 references
- [`conf/modules/lofreq.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/lofreq.config#L22) — 2 references
- [`conf/modules/ngscheckmate.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/ngscheckmate.config#L8) — 2 references
- [`conf/modules/parabricks_haplotypecaller.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/parabricks_haplotypecaller.config#L20) — 2 references
- [`conf/modules/prepare_recalibration.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/prepare_recalibration.config#L20) — 2 references
- [`conf/modules/sentieon_dedup.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/sentieon_dedup.config#L32) — 2 references
- [`conf/modules/sentieon_tnscope.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/sentieon_tnscope.config#L24) — 2 references
- [`conf/modules/strelka.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/strelka.config#L22) — 2 references
- [`conf/modules/ascat.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/ascat.config#L31) — 1 reference
- [`conf/modules/contamination.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/contamination.config#L9) — 1 reference
- [`conf/modules/manta.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/manta.config#L20) — 1 reference
- [`conf/modules/msisensor2.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/msisensor2.config#L19) — 1 reference
- [`conf/modules/msisensorpro.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/msisensorpro.config#L18) — 1 reference
- [`conf/modules/trimming.config`](https://github.com/nf-core/sarek/blob/7e455477b7b55f89a5adad02434d42dc51eaaaea/conf/modules/trimming.config#L35) — 1 reference
