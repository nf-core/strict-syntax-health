# Nextflow lint results

- Generated: 2026-05-09T00:35:31.421306008Z
- Nextflow version: 26.04.0
- Summary: 15 warnings

## :warning: Warnings

- Warning: `modules/nf-core/custom/gtffilter/main.nf:24:5`: Variable was declared but not used

  ```nextflow
      args   = task.ext.args ?: ''
      ^^^^
  ```

- Warning: `modules/nf-core/ea-utils/gtf2bed/main.nf:22:5`: Variable was declared but not used

  ```nextflow
      args   = task.ext.args ?: ''
      ^^^^
  ```

- Warning: `subworkflows/local/multiqc_rnaseq/main.nf:359:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
  def strandSummaryCells(meta, provided, status, salmon, rseqc) {
                         ^^^^
  ```

- Warning: `subworkflows/local/multiqc_rnaseq/main.nf:391:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def data = rows.toSorted { it[0].id }.collectEntries { row ->
                                 ^^
  ```

- Warning: `subworkflows/local/multiqc_rnaseq/main.nf:431:21`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      rows.toSorted { it[0].id }.each { row ->
                      ^^
  ```

- Warning: `subworkflows/local/prepare_genome_indices/main.nf:219:120`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ch_bowtie2_index = UNTAR_BOWTIE2_INDEX ([ [:], file(bowtie2_index, checkIfExists: true) ]).untar.map { meta, index -> index }
                                                                                                                         ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome_indices/main.nf:229:62`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_bowtie2_index = BOWTIE2_BUILD.out.index.map { meta, index -> index }
                                                               ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome_references/main.nf:174:79`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_transcript_fasta = GFFREAD_TRANSCRIPTS.out.gffread_fasta.map { meta, fasta_file -> fasta_file }
                                                                                ^^^^
  ```

- Warning: `subworkflows/nf-core/bam_dedup_umi/main.nf:129:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { row -> [row[0], row.drop(1).findAll { it != null }.collectMany { e -> (e instanceof List) ? e : [e] }] }
                                                       ^^
  ```

- Warning: `subworkflows/nf-core/bam_markduplicates_picard/main.nf:29:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { row -> [row[0], row.drop(1).findAll { it != null }.collectMany { e -> (e instanceof List) ? e : [e] }] }
                                                       ^^
  ```

- Warning: `subworkflows/nf-core/bam_qc_rnaseq/main.nf:25:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def rseqc_modules = tools.findAll { it.startsWith('rseqc_') }.collect { it.replace('rseqc_', '') }
                                          ^^
  ```

- Warning: `subworkflows/nf-core/bam_qc_rnaseq/main.nf:25:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def rseqc_modules = tools.findAll { it.startsWith('rseqc_') }.collect { it.replace('rseqc_', '') }
                                                                              ^^
  ```

- Warning: `subworkflows/nf-core/bam_qc_rnaseq/main.nf:85:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_qc_rnaseq/main.nf:113:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { row -> [row[0], row.drop(1).findAll { it != null }.collectMany { e -> (e instanceof List) ? e : [e] }] }
                                                       ^^
  ```

- Warning: `subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/main.nf:426:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { row -> [row[0], row.drop(1).findAll { it != null }.collectMany { e -> (e instanceof List) ? e : [e] }] }
                                                       ^^
  ```
