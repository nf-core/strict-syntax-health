# Workflow outputs migration: sarek

- Generated: 2026-06-16T14:33:29.286048+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:388`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/main.nf#L388)

  ```nextflow
  output {
  ```

## Legacy `publishDir` references

Found 187 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules/aligner.config:37`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/aligner.config#L37)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/aligner.config:76`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/aligner.config#L76)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/aligner_parabricks.config:27`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/aligner_parabricks.config#L27)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/aligner_parabricks.config:37`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/aligner_parabricks.config#L37)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/aligner_parabricks.config:46`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/aligner_parabricks.config#L46)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/aligner_parabricks.config:56`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/aligner_parabricks.config#L56)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/alignment_to_fastq.config:21`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/alignment_to_fastq.config#L21)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/alignment_to_fastq.config:30`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/alignment_to_fastq.config#L30)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/alignment_to_fastq.config:39`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/alignment_to_fastq.config#L39)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/alignment_to_fastq.config:48`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/alignment_to_fastq.config#L48)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/alignment_to_fastq.config:57`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/alignment_to_fastq.config#L57)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/alignment_to_fastq.config:66`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/alignment_to_fastq.config#L66)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/alignment_to_fastq.config:74`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/alignment_to_fastq.config#L74)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/alignment_to_fastq.config:80`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/alignment_to_fastq.config#L80)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/annotate.config:22`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/annotate.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/annotate.config:49`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/annotate.config#L49)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/annotate.config:67`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/annotate.config#L67)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/annotate.config:77`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/annotate.config#L77)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/annotate.config:85`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/annotate.config#L85)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/annotate.config:114`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/annotate.config#L114)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/annotate.config:122`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/annotate.config#L122)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/ascat.config:31`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/ascat.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/cnvkit.config:21`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/cnvkit.config#L21)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/cnvkit.config:30`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/cnvkit.config#L30)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/cnvkit.config:51`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/cnvkit.config#L51)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/cnvkit.config:61`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/cnvkit.config#L61)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/contamination.config:7`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/contamination.config#L7)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/controlfreec.config:19`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/controlfreec.config#L19)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/controlfreec.config:28`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/controlfreec.config#L28)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/controlfreec.config:37`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/controlfreec.config#L37)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/controlfreec.config:46`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/controlfreec.config#L46)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/controlfreec.config:54`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/controlfreec.config#L54)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/deepvariant.config:25`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/deepvariant.config#L25)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/deepvariant.config:35`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/deepvariant.config#L35)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/download_cache.config:21`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/download_cache.config#L21)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/download_cache.config:31`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/download_cache.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/freebayes.config:20`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/freebayes.config#L20)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/freebayes.config:32`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/freebayes.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/freebayes.config:39`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/freebayes.config#L39)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/freebayes.config:48`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/freebayes.config#L48)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/freebayes.config:58`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/freebayes.config#L58)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/freebayes.config:66`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/freebayes.config#L66)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/haplotypecaller.config:25`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/haplotypecaller.config#L25)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/haplotypecaller.config:35`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/haplotypecaller.config#L35)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/haplotypecaller.config:43`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/haplotypecaller.config#L43)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/haplotypecaller.config:52`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/haplotypecaller.config#L52)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/haplotypecaller.config:61`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/haplotypecaller.config#L61)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/indexcov.config:8`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/indexcov.config#L8)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/indexcov.config:15`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/indexcov.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/joint_germline.config:23`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/joint_germline.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/joint_germline.config:30`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/joint_germline.config#L30)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/joint_germline.config:37`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/joint_germline.config#L37)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/joint_germline.config:44`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/joint_germline.config#L44)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/joint_germline.config:54`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/joint_germline.config#L54)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/joint_germline.config:62`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/joint_germline.config#L62)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/joint_germline.config:70`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/joint_germline.config#L70)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/joint_germline.config:78`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/joint_germline.config#L78)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/lofreq.config:22`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/lofreq.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/lofreq.config:36`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/lofreq.config#L36)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/manta.config:20`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/manta.config#L20)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/markduplicates.config:21`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/markduplicates.config#L21)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/markduplicates.config:37`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/markduplicates.config#L37)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/markduplicates.config:49`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/markduplicates.config#L49)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/markduplicates.config:69`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/markduplicates.config#L69)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/markduplicates.config:97`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/markduplicates.config#L97)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/markduplicates.config:114`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/markduplicates.config#L114)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/modules.config:19`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/modules.config#L19)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/modules.config:33`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/modules.config#L33)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/modules.config:45`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/modules.config#L45)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/modules.config:54`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/modules.config#L54)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/modules.config:71`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/modules.config#L71)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/modules.config:85`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/modules.config#L85)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/modules.config:96`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/modules.config#L96)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/modules.config:106`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/modules.config#L106)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/mpileup.config:19`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/mpileup.config#L19)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/mpileup.config:29`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/mpileup.config#L29)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/mpileup.config:39`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/mpileup.config#L39)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/mpileup.config:48`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/mpileup.config#L48)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/msisensor2.config:19`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/msisensor2.config#L19)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/msisensorpro.config:18`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/msisensorpro.config#L18)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/muse.config:22`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/muse.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/muse.config:33`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/muse.config#L33)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/muse.config:49`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/muse.config#L49)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/mutect2.config:22`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/mutect2.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/mutect2.config:39`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/mutect2.config#L39)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/mutect2.config:48`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/mutect2.config#L48)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/mutect2.config:58`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/mutect2.config#L58)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/mutect2.config:67`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/mutect2.config#L67)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/mutect2.config:76`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/mutect2.config#L76)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/mutect2.config:85`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/mutect2.config#L85)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/mutect2.config:94`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/mutect2.config#L94)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/ngscheckmate.config:8`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/ngscheckmate.config#L8)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/ngscheckmate.config:17`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/ngscheckmate.config#L17)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/post_variant_calling.config:24`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/post_variant_calling.config#L24)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/post_variant_calling.config:32`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/post_variant_calling.config#L32)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules/post_variant_calling.config:37`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/post_variant_calling.config#L37)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules/post_variant_calling.config:46`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/post_variant_calling.config#L46)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/post_variant_calling.config:54`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/post_variant_calling.config#L54)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/post_variant_calling.config:64`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/post_variant_calling.config#L64)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules/post_variant_calling.config:71`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/post_variant_calling.config#L71)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/post_variant_calling.config:80`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/post_variant_calling.config#L80)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/post_variant_calling.config:89`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/post_variant_calling.config#L89)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules/post_variant_calling.config:95`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/post_variant_calling.config#L95)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:18`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/prepare_genome.config#L18)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:27`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/prepare_genome.config#L27)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:36`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/prepare_genome.config#L36)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_genome.config:46`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/prepare_genome.config#L46)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:57`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/prepare_genome.config#L57)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:66`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/prepare_genome.config#L66)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:75`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/prepare_genome.config#L75)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_genome.config:84`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/prepare_genome.config#L84)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:93`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/prepare_genome.config#L93)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:102`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/prepare_genome.config#L102)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_genome.config:111`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/prepare_genome.config#L111)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_genome.config:120`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/prepare_genome.config#L120)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_genome.config:129`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/prepare_genome.config#L129)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_genome.config:138`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/prepare_genome.config#L138)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_genome.config:147`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/prepare_genome.config#L147)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_genome.config:156`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/prepare_genome.config#L156)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_genome.config:165`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/prepare_genome.config#L165)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_genome.config:172`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/prepare_genome.config#L172)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_genome.config:181`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/prepare_genome.config#L181)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_intervals.config:24`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/prepare_intervals.config#L24)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_intervals.config:33`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/prepare_intervals.config#L33)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_intervals.config:43`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/prepare_intervals.config#L43)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_recalibration.config:21`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/prepare_recalibration.config#L21)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/prepare_recalibration.config:32`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/prepare_recalibration.config#L32)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/recalibrate.config:24`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/recalibrate.config#L24)

  ```nextflow
  publishDir       = [[
  ```

- [`conf/modules/recalibrate.config:46`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/recalibrate.config#L46)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/recalibrate.config:55`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/recalibrate.config#L55)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/recalibrate.config:65`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/recalibrate.config#L65)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/recalibrate.config:74`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/recalibrate.config#L74)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/sentieon_dedup.config:30`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/sentieon_dedup.config#L30)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/sentieon_dedup.config:58`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/sentieon_dedup.config#L58)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/sentieon_dnascope.config:21`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/sentieon_dnascope.config#L21)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/sentieon_dnascope.config:31`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/sentieon_dnascope.config#L31)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/sentieon_dnascope.config:40`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/sentieon_dnascope.config#L40)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/sentieon_dnascope.config:49`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/sentieon_dnascope.config#L49)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/sentieon_haplotyper.config:21`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/sentieon_haplotyper.config#L21)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/sentieon_haplotyper.config:31`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/sentieon_haplotyper.config#L31)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/sentieon_haplotyper.config:40`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/sentieon_haplotyper.config#L40)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/sentieon_haplotyper.config:50`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/sentieon_haplotyper.config#L50)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/sentieon_joint_germline.config:21`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/sentieon_joint_germline.config#L21)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/sentieon_joint_germline.config:28`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/sentieon_joint_germline.config#L28)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/sentieon_joint_germline.config:35`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/sentieon_joint_germline.config#L35)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/sentieon_joint_germline.config:45`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/sentieon_joint_germline.config#L45)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/sentieon_joint_germline.config:53`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/sentieon_joint_germline.config#L53)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/sentieon_joint_germline.config:63`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/sentieon_joint_germline.config#L63)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/sentieon_joint_germline.config:72`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/sentieon_joint_germline.config#L72)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/sentieon_tnscope.config:24`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/sentieon_tnscope.config#L24)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules/sentieon_tnscope.config:34`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/sentieon_tnscope.config#L34)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/strelka.config:22`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/strelka.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/strelka.config:31`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/strelka.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/tiddit.config:22`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/tiddit.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/tiddit.config:31`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/tiddit.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/tiddit.config:51`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/tiddit.config#L51)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/trimming.config:32`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/trimming.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/umi.config:22`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/umi.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/umi.config:31`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/umi.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/umi.config:41`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/umi.config#L41)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/umi.config:50`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/umi.config#L50)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/umi.config:59`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/umi.config#L59)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/umi.config:66`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/umi.config#L66)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/umi.config:77`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/umi.config#L77)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/umi.config:85`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/umi.config#L85)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/varlociraptor.config:22`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/varlociraptor.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/varlociraptor.config:33`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/varlociraptor.config#L33)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/varlociraptor.config:41`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/varlociraptor.config#L41)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/varlociraptor.config:48`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/varlociraptor.config#L48)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/varlociraptor.config:55`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/varlociraptor.config#L55)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/varlociraptor.config:62`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/varlociraptor.config#L62)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/varlociraptor.config:80`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/varlociraptor.config#L80)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/varlociraptor.config:88`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/varlociraptor.config#L88)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/varlociraptor.config:98`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/varlociraptor.config#L98)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/varlociraptor.config:106`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/varlociraptor.config#L106)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/varlociraptor.config:118`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/varlociraptor.config#L118)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/varlociraptor.config:125`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/varlociraptor.config#L125)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/varlociraptor.config:133`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/varlociraptor.config#L133)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/varlociraptor.config:143`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/varlociraptor.config#L143)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/varlociraptor.config:152`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/varlociraptor.config#L152)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/varlociraptor.config:159`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/varlociraptor.config#L159)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/varlociraptor.config:166`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/varlociraptor.config#L166)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/varlociraptor.config:174`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/varlociraptor.config#L174)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/varlociraptor.config:181`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/varlociraptor.config#L181)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/varlociraptor.config:193`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/varlociraptor.config#L193)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/varlociraptor.config:201`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/conf/modules/varlociraptor.config#L201)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/local/channel_markduplicates_create_csv/main.nf:22`](https://github.com/nf-core/sarek/blob/84c6613f340f20d11f9358e2a55d8d87bd8ad384/subworkflows/local/channel_markduplicates_create_csv/main.nf#L22)

  ```nextflow
  // GATK4_MARKDUPLICATES publishDir renames it to *.md.bam.bai on disk, so use
  ```
