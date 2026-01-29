# Nextflow lint results

- Generated: 2026-01-29T00:20:02.465745528Z
- Nextflow version: 25.12.0-edge
- Summary: 15 warnings

## :warning: Warnings

- Warning: `modules/nf-core/quast/main.nf:48:9`: Variable was declared but not used

  ```nextflow
      def args      = task.ext.args   ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/quast/main.nf:50:9`: Variable was declared but not used

  ```nextflow
      def features  = gff             ? "--features $gff" : ''
          ^^^^^^^^
  ```

- Warning: `modules/nf-core/quast/main.nf:51:9`: Variable was declared but not used

  ```nextflow
      def reference = fasta           ? "-r $fasta" : ''
          ^^^^^^^^^
  ```

- Warning: `modules/nf-core/toulligqc/main.nf:46:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_trim_fastp_fastqc/main.nf:34:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_trim_fastp_fastqc/main.nf:37:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_reads_only = ch_reads.map { meta, reads, adapter_fasta -> [ meta, reads ] }
                                                  ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_trim_fastp_fastqc/main.nf:39:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_fastqc_raw_html = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_trim_fastp_fastqc/main.nf:40:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_fastqc_raw_zip  = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_trim_fastp_fastqc/main.nf:50:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_trim_json         = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_trim_fastp_fastqc/main.nf:51:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_trim_html         = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_trim_fastp_fastqc/main.nf:52:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_trim_log          = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_trim_fastp_fastqc/main.nf:53:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_trim_reads_fail   = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_trim_fastp_fastqc/main.nf:54:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_trim_reads_merged = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_trim_fastp_fastqc/main.nf:55:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_fastqc_trim_html  = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_trim_fastp_fastqc/main.nf:56:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_fastqc_trim_zip   = Channel.empty()
                             ^^^^^^^
  ```
