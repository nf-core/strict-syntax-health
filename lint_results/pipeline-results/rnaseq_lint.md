# Nextflow lint results

- Generated: 2026-04-24T00:32:59.833674076Z
- Nextflow version: 26.03.3-edge
- Summary: 26 warnings

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

- Warning: `subworkflows/local/multiqc_rnaseq/main.nf:134:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              [mqc_default_config, dynamic_config, mqc_custom_config].findAll { it },
                                                                                ^^
  ```

- Warning: `subworkflows/local/multiqc_rnaseq/main.nf:173:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          .findAll { it != null }
                                     ^^
  ```

- Warning: `subworkflows/local/multiqc_rnaseq/main.nf:358:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
  def strandSummaryCells(meta, provided, status, salmon, rseqc) {
                         ^^^^
  ```

- Warning: `subworkflows/local/multiqc_rnaseq/main.nf:439:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          pconfig.data_labels = labels.collect { [name: it, ylab: pconfig.ylab] }
                                                        ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:195:79`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_transcript_fasta = GFFREAD_TRANSCRIPTS.out.gffread_fasta.map { meta, fasta_file -> fasta_file }
                                                                                ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:392:120`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ch_bowtie2_index = UNTAR_BOWTIE2_INDEX ([ [:], file(bowtie2_index, checkIfExists: true) ]).untar.map { meta, index -> index }
                                                                                                                         ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:402:62`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_bowtie2_index = BOWTIE2_BUILD.out.index.map { meta, index -> index }
                                                               ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_rnaseq_pipeline/main.nf:706:61`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ? params.rseqc_modules.split(',').collect { it.trim().toLowerCase() }
                                                              ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_rnaseq_pipeline/main.nf:711:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              rseqc_modules.each { tools << "rseqc_${it}" }
                                                     ^^
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

- Warning: `subworkflows/nf-core/quant_tximport_summarizedexperiment/main.nf:33:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, results -> [ [:], results ] }
                 ^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```

- Warning: `workflows/rnaseq/main.nf:121:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def collapseAgg = { row -> [row[0].id, row.drop(1).findAll { it != null }.collectMany { e -> (e instanceof List) ? e : [e] }] }
                                                                   ^^
  ```

- Warning: `workflows/rnaseq/main.nf:554:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def rseqc_modules = qc_tools.findAll { it.startsWith('rseqc_') }.collect { it.replace('rseqc_', '') }
                                             ^^
  ```

- Warning: `workflows/rnaseq/main.nf:554:80`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def rseqc_modules = qc_tools.findAll { it.startsWith('rseqc_') }.collect { it.replace('rseqc_', '') }
                                                                                 ^^
  ```

- Warning: `workflows/rnaseq/main.nf:607:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      def ie = (files instanceof List ? files : [files]).find { it.name.endsWith('.infer_experiment.txt') }
                                                                                ^^
  ```

- Warning: `workflows/rnaseq/main.nf:610:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .filter { it != null }
                            ^^
  ```

- Warning: `workflows/rnaseq/main.nf:620:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  Channel.value([ [:], ch_biotypes_header_multiqc ]),
                  ^^^^^^^
  ```
