# Workflow outputs migration: rnaseq

- Generated: 2026-06-16T14:31:57.340098+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 118 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules/align_bowtie2.config:39`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/align_bowtie2.config#L39)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/align_hisat2.config:17`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/align_hisat2.config#L17)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/align_star.config:138`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/align_star.config#L138)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/alignment.config:8`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/alignment.config#L8)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/alignment.config:24`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/alignment.config#L24)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bbsplit.config:4`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/bbsplit.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bigwig.config:22`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/bigwig.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bigwig.config:52`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/bigwig.config#L52)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bracken.config:4`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/bracken.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/cat_fastq.config:3`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/cat_fastq.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/deseq2_qc.config:14`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/deseq2_qc.config#L14)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/dupradar.config:3`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/dupradar.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/fastp.config:5`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/fastp.config#L5)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/fastp.config:14`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/fastp.config#L14)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/fastp.config:22`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/fastp.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/fastp.config:49`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/fastp.config#L49)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/featurecounts.config:8`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/featurecounts.config#L8)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/kraken2.config:6`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/kraken2.config#L6)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/markduplicates.config:5`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/markduplicates.config#L5)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/markduplicates.config:22`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/markduplicates.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/markduplicates.config:32`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/markduplicates.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/multiqc.config:7`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/multiqc.config#L7)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/multiqc_custom_biotype.config:3`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/multiqc_custom_biotype.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:3`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/prepare_genome.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:15`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/prepare_genome.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:24`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/prepare_genome.config#L24)

  ```nextflow
  publishDir = []
  ```

- [`conf/modules/prepare_genome.config:50`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/prepare_genome.config#L50)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:62`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/prepare_genome.config#L62)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:74`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/prepare_genome.config#L74)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:82`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/prepare_genome.config#L82)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:90`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/prepare_genome.config#L90)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:102`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/prepare_genome.config#L102)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:111`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/prepare_genome.config#L111)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:119`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/prepare_genome.config#L119)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:127`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/prepare_genome.config#L127)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:136`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/prepare_genome.config#L136)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:144`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/prepare_genome.config#L144)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:153`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/prepare_genome.config#L153)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:161`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/prepare_genome.config#L161)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:171`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/prepare_genome.config#L171)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_genome.config:180`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/prepare_genome.config#L180)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/preseq.config:4`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/preseq.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/qc_trim_filter.config:5`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/qc_trim_filter.config#L5)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/qc_trim_filter.config:12`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/qc_trim_filter.config#L12)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/qc_trim_filter.config:19`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/qc_trim_filter.config#L19)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/qc_trim_filter.config:26`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/qc_trim_filter.config#L26)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/qc_trim_filter.config:39`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/qc_trim_filter.config#L39)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/qc_trim_filter.config:66`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/qc_trim_filter.config#L66)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/qc_trim_filter.config:77`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/qc_trim_filter.config#L77)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/qc_trim_filter.config:97`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/qc_trim_filter.config#L97)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/qc_trim_filter.config:107`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/qc_trim_filter.config#L107)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/qc_trim_filter.config:125`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/qc_trim_filter.config#L125)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/qc_trim_filter.config:143`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/qc_trim_filter.config#L143)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/qc_trim_filter.config:150`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/qc_trim_filter.config#L150)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/qualimap.config:5`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/qualimap.config#L5)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/qualimap.config:12`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/qualimap.config#L12)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/quantify_bam_salmon.config:8`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/quantify_bam_salmon.config#L8)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/quantify_bam_salmon.config:16`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/quantify_bam_salmon.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/quantify_bam_salmon.config:28`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/quantify_bam_salmon.config#L28)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/quantify_bam_salmon.config:48`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/quantify_bam_salmon.config#L48)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/quantify_bam_salmon.config:58`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/quantify_bam_salmon.config#L58)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/quantify_bam_salmon.config:78`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/quantify_bam_salmon.config#L78)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/quantify_bam_salmon.config:88`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/quantify_bam_salmon.config#L88)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/quantify_bam_salmon.config:105`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/quantify_bam_salmon.config#L105)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/quantify_bam_salmon.config:128`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/quantify_bam_salmon.config#L128)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/quantify_bam_salmon.config:144`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/quantify_bam_salmon.config#L144)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/quantify_bam_salmon.config:154`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/quantify_bam_salmon.config#L154)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/quantify_pseudo_alignment.config:8`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/quantify_pseudo_alignment.config#L8)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/quantify_pseudo_alignment.config:17`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/quantify_pseudo_alignment.config#L17)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/quantify_pseudo_alignment.config:25`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/quantify_pseudo_alignment.config#L25)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/quantify_pseudo_alignment.config:37`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/quantify_pseudo_alignment.config#L37)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/quantify_pseudo_alignment.config:60`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/quantify_pseudo_alignment.config#L60)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/quantify_rsem.config:7`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/quantify_rsem.config#L7)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/quantify_rsem.config:22`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/quantify_rsem.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/quantify_rsem.config:29`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/quantify_rsem.config#L29)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/quantify_rsem.config:41`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/quantify_rsem.config#L41)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/rseqc.config:3`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/rseqc.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/rseqc.config:10`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/rseqc.config#L10)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/rseqc.config:17`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/rseqc.config#L17)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/rseqc.config:47`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/rseqc.config#L47)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/rseqc.config:62`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/rseqc.config#L62)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/rseqc.config:82`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/rseqc.config#L82)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/rseqc.config:89`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/rseqc.config#L89)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/rseqc.config:109`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/rseqc.config#L109)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/rustqc.config:13`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/rustqc.config#L13)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/sortmerna.config:4`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/sortmerna.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/strandedness.config:5`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/strandedness.config#L5)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/strandedness.config:12`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/strandedness.config#L12)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/stringtie.config:4`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/stringtie.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/stringtie.config:16`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/stringtie.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/stringtie.config:27`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/stringtie.config#L27)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/sylph.config:7`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/sylph.config#L7)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/sylphtax.config:3`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/sylphtax.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/trimgalore.config:5`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/trimgalore.config#L5)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/trimgalore.config:33`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/trimgalore.config#L33)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/trimgalore.config:60`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/trimgalore.config#L60)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/umi_dedup.config:26`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/umi_dedup.config#L26)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules/umi_dedup.config:31`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/umi_dedup.config#L31)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules/umi_dedup.config:43`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/umi_dedup.config#L43)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/umi_dedup.config:66`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/umi_dedup.config#L66)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/umi_dedup.config:84`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/umi_dedup.config#L84)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/umi_dedup.config:94`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/conf/modules/umi_dedup.config#L94)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/rsem/calculateexpression/tests/alignment.config:3`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/modules/nf-core/rsem/calculateexpression/tests/alignment.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`modules/nf-core/rsem/calculateexpression/tests/nextflow.config:3`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/modules/nf-core/rsem/calculateexpression/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`modules/nf-core/rseqc/bamstat/tests/nextflow.config:3`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/modules/nf-core/rseqc/bamstat/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`modules/nf-core/rseqc/inferexperiment/tests/nextflow.config:3`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/modules/nf-core/rseqc/inferexperiment/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`modules/nf-core/subread/featurecounts/tests/nextflow.config:3`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`modules/nf-core/umitools/extract/tests/nextflow.config:3`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/modules/nf-core/umitools/extract/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`nextflow.config:159`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/nextflow.config#L159)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```

- [`nextflow.config:174`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/nextflow.config#L174)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/local/align_star/tests/nextflow.extra_args.config:24`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/subworkflows/local/align_star/tests/nextflow.extra_args.config#L24)

  ```nextflow
  // Disable publishDir during tests
  ```

- [`subworkflows/local/align_star/tests/nextflow.extra_args.config:26`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/subworkflows/local/align_star/tests/nextflow.extra_args.config#L26)

  ```nextflow
  publishDir = []
  ```

- [`subworkflows/local/align_star/tests/nextflow.rg.config:24`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/subworkflows/local/align_star/tests/nextflow.rg.config#L24)

  ```nextflow
  // Disable publishDir during tests
  ```

- [`subworkflows/local/align_star/tests/nextflow.rg.config:26`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/subworkflows/local/align_star/tests/nextflow.rg.config#L26)

  ```nextflow
  publishDir = []
  ```

- [`subworkflows/nf-core/bedgraph_bedclip_bedgraphtobigwig/tests/nextflow.config:3`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/subworkflows/nf-core/bedgraph_bedclip_bedgraphtobigwig/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/tests/nextflow.config:22`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/tests/nextflow.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/tests/nextflow.config:29`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/tests/nextflow.config#L29)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/nf-core/fastq_subsample_fq_salmon/tests/nextflow.config:3`](https://github.com/nf-core/rnaseq/blob/61651dc4b5842ca0bd6394a22d42b326d50daa2f/subworkflows/nf-core/fastq_subsample_fq_salmon/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```
