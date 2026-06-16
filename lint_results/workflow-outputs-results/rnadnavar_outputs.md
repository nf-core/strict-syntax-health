# Workflow outputs migration: rnadnavar

- Generated: 2026-06-16T14:31:20.516680+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 97 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/alignment/alignment_to_fastq.config:21`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/alignment/alignment_to_fastq.config#L21)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/alignment/alignment_to_fastq.config:30`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/alignment/alignment_to_fastq.config#L30)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/alignment/alignment_to_fastq.config:39`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/alignment/alignment_to_fastq.config#L39)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/alignment/alignment_to_fastq.config:48`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/alignment/alignment_to_fastq.config#L48)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/alignment/alignment_to_fastq.config:57`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/alignment/alignment_to_fastq.config#L57)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/alignment/alignment_to_fastq.config:66`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/alignment/alignment_to_fastq.config#L66)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/alignment/alignment_to_fastq.config:74`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/alignment/alignment_to_fastq.config#L74)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/alignment/alignment_to_fastq.config:80`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/alignment/alignment_to_fastq.config#L80)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/alignment/bam_align.config:35`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/alignment/bam_align.config#L35)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/alignment/bam_align.config:62`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/alignment/bam_align.config#L62)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/alignment/bam_align.config:87`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/alignment/bam_align.config#L87)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/alignment/bam_align.config:117`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/alignment/bam_align.config#L117)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/alignment/bam_align.config:143`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/alignment/bam_align.config#L143)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/alignment/bam_align.config:168`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/alignment/bam_align.config#L168)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/alignment/bam_align.config:180`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/alignment/bam_align.config#L180)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/alignment/bam_align.config:196`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/alignment/bam_align.config#L196)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/alignment/bam_align.config:207`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/alignment/bam_align.config#L207)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/alignment/bam_align.config:217`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/alignment/bam_align.config#L217)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/annotate/annotate.config:31`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/annotate/annotate.config#L31)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/annotate/annotate.config:47`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/annotate/annotate.config#L47)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/consensus/vcf_consensus.config:30`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/consensus/vcf_consensus.config#L30)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/consensus/vcf_consensus.config:40`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/consensus/vcf_consensus.config#L40)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/filtering/maf_filtering.config:25`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/filtering/maf_filtering.config#L25)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/filtering/maf_filtering.config:43`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/filtering/maf_filtering.config#L43)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/gatk4_preprocessing/markduplicates.config:28`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/gatk4_preprocessing/markduplicates.config#L28)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/gatk4_preprocessing/markduplicates.config:40`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/gatk4_preprocessing/markduplicates.config#L40)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/gatk4_preprocessing/markduplicates.config:53`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/gatk4_preprocessing/markduplicates.config#L53)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/gatk4_preprocessing/markduplicates.config:70`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/gatk4_preprocessing/markduplicates.config#L70)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/gatk4_preprocessing/markduplicates.config:81`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/gatk4_preprocessing/markduplicates.config#L81)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/gatk4_preprocessing/prepare_recalibration.config:21`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/gatk4_preprocessing/prepare_recalibration.config#L21)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/gatk4_preprocessing/prepare_recalibration.config:32`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/gatk4_preprocessing/prepare_recalibration.config#L32)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/gatk4_preprocessing/recalibrate.config:20`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/gatk4_preprocessing/recalibrate.config#L20)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/gatk4_preprocessing/recalibrate.config:32`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/gatk4_preprocessing/recalibrate.config#L32)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/gatk4_preprocessing/recalibrate.config:41`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/gatk4_preprocessing/recalibrate.config#L41)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/gatk4_preprocessing/recalibrate.config:52`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/gatk4_preprocessing/recalibrate.config#L52)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/gatk4_preprocessing/splitncigarreads.config:21`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/gatk4_preprocessing/splitncigarreads.config#L21)

  ```nextflow
  publishDir     = [
  ```

- [`conf/modules/gatk4_preprocessing/splitncigarreads.config:33`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/gatk4_preprocessing/splitncigarreads.config#L33)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/gatk4_preprocessing/splitncigarreads.config:42`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/gatk4_preprocessing/splitncigarreads.config#L42)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/gatk4_preprocessing/splitncigarreads.config:54`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/gatk4_preprocessing/splitncigarreads.config#L54)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/gatk4_preprocessing/splitncigarreads.config:65`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/gatk4_preprocessing/splitncigarreads.config#L65)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/modules.config:15`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/normalize/vt.config:21`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/normalize/vt.config#L21)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/normalize/vt.config:39`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/normalize/vt.config#L39)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_realignment/extract_reads_id.config:21`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/prepare_realignment/extract_reads_id.config#L21)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_realignment/extract_reads_id.config:31`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/prepare_realignment/extract_reads_id.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_realignment/filtersamreads.config:21`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/prepare_realignment/filtersamreads.config#L21)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_resources/prepare_cache.config:22`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/prepare_resources/prepare_cache.config#L22)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_resources/prepare_genome.config:20`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/prepare_resources/prepare_genome.config#L20)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_resources/prepare_genome.config:30`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/prepare_resources/prepare_genome.config#L30)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_resources/prepare_genome.config:40`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/prepare_resources/prepare_genome.config#L40)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_resources/prepare_genome.config:58`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/prepare_resources/prepare_genome.config#L58)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_resources/prepare_genome.config:68`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/prepare_resources/prepare_genome.config#L68)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_resources/prepare_genome.config:78`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/prepare_resources/prepare_genome.config#L78)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_resources/prepare_genome.config:88`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/prepare_resources/prepare_genome.config#L88)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_resources/prepare_genome.config:98`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/prepare_resources/prepare_genome.config#L98)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_resources/prepare_genome.config:108`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/prepare_resources/prepare_genome.config#L108)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_resources/prepare_genome.config:118`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/prepare_resources/prepare_genome.config#L118)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_resources/prepare_genome.config:128`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/prepare_resources/prepare_genome.config#L128)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_resources/prepare_intervals.config:19`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/prepare_resources/prepare_intervals.config#L19)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_resources/prepare_intervals.config:28`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/prepare_resources/prepare_intervals.config#L28)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_resources/prepare_intervals.config:37`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/prepare_resources/prepare_intervals.config#L37)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_resources/prepare_intervals.config:48`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/prepare_resources/prepare_intervals.config#L48)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_resources/prepare_intervals.config:57`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/prepare_resources/prepare_intervals.config#L57)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_resources/prepare_intervals.config:67`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/prepare_resources/prepare_intervals.config#L67)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/quality_control/quality_control.config:20`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/quality_control/quality_control.config#L20)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/quality_control/quality_control.config:31`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/quality_control/quality_control.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/quality_control/quality_control.config:44`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/quality_control/quality_control.config#L44)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/quality_control/quality_control.config:61`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/quality_control/quality_control.config#L61)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/quality_control/quality_control.config:78`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/quality_control/quality_control.config#L78)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/quality_control/quality_control.config:88`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/quality_control/quality_control.config#L88)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/quality_control/quality_control.config:99`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/quality_control/quality_control.config#L99)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/quality_control/quality_control.config:109`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/quality_control/quality_control.config#L109)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/quality_control/quality_control.config:132`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/quality_control/quality_control.config#L132)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules/quality_control/quality_control.config:142`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/quality_control/quality_control.config#L142)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules/quality_control/quality_control.config:152`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/quality_control/quality_control.config#L152)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules/quality_control/quality_control.config:169`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/quality_control/quality_control.config#L169)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules/quality_control/trimming.config:28`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/quality_control/trimming.config#L28)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/variant_calling/mutect2.config:25`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/variant_calling/mutect2.config#L25)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/variant_calling/mutect2.config:35`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/variant_calling/mutect2.config#L35)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/variant_calling/mutect2.config:51`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/variant_calling/mutect2.config#L51)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/variant_calling/mutect2.config:61`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/variant_calling/mutect2.config#L61)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/variant_calling/mutect2.config:70`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/variant_calling/mutect2.config#L70)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/variant_calling/mutect2.config:79`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/variant_calling/mutect2.config#L79)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/variant_calling/mutect2.config:88`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/variant_calling/mutect2.config#L88)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/variant_calling/mutect2.config:97`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/variant_calling/mutect2.config#L97)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/variant_calling/mutect2.config:107`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/variant_calling/mutect2.config#L107)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/variant_calling/sage.config:27`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/variant_calling/sage.config#L27)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/variant_calling/sage.config:34`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/variant_calling/sage.config#L34)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/variant_calling/sage.config:43`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/variant_calling/sage.config#L43)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/variant_calling/strelka.config:23`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/variant_calling/strelka.config#L23)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/variant_calling/strelka.config:33`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/variant_calling/strelka.config#L33)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/variant_calling/variant_calling.config:21`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/conf/modules/variant_calling/variant_calling.config#L21)

  ```nextflow
  publishDir       = [
  ```

- [`modules/nf-core/gatk4/variantrecalibrator/tests/AS.config:3`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/modules/nf-core/gatk4/variantrecalibrator/tests/AS.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`modules/nf-core/gatk4/variantrecalibrator/tests/noAS.config:3`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/modules/nf-core/gatk4/variantrecalibrator/tests/noAS.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`subworkflows/nf-core/fastq_align_star/tests/nextflow.config:3`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/subworkflows/nf-core/fastq_align_star/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config:3`](https://github.com/nf-core/rnadnavar/blob/26df4e3c87388298a607231049cf8f59433c97c9/subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```
