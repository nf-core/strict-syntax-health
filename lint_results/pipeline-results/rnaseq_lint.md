# Nextflow lint results

- Generated: 2026-04-18T00:28:31.107500641Z
- Nextflow version: 26.03.2-edge
- Summary: 19 warnings

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

- Warning: `subworkflows/local/multiqc_rnaseq/main.nf:78:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      [mqc_default_config, dyn, mqc_custom_config].findAll { it },
                                                                             ^^
  ```

- Warning: `subworkflows/local/multiqc_rnaseq/main.nf:101:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      [mqc_default_config, dyn, mqc_custom_config].findAll { it },
                                                                             ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:198:79`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_transcript_fasta = GFFREAD_TRANSCRIPTS.out.gffread_fasta.map { meta, fasta_file -> fasta_file }
                                                                                ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:384:120`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ch_bowtie2_index = UNTAR_BOWTIE2_INDEX ([ [:], file(bowtie2_index, checkIfExists: true) ]).untar.map { meta, index -> index }
                                                                                                                         ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:394:62`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_bowtie2_index = BOWTIE2_BUILD.out.index.map { meta, index -> index }
                                                               ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_rnaseq_pipeline/main.nf:761:61`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ? params.rseqc_modules.split(',').collect { it.trim().toLowerCase() }
                                                              ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_rnaseq_pipeline/main.nf:766:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              rseqc_modules.each { tools << "rseqc_${it}" }
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

- Warning: `workflows/rnaseq/main.nf:510:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def rseqc_modules = qc_tools.findAll { it.startsWith('rseqc_') }.collect { it.replace('rseqc_', '') }
                                             ^^
  ```

- Warning: `workflows/rnaseq/main.nf:510:80`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def rseqc_modules = qc_tools.findAll { it.startsWith('rseqc_') }.collect { it.replace('rseqc_', '') }
                                                                                 ^^
  ```

- Warning: `workflows/rnaseq/main.nf:545:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      def ie = (files instanceof List ? files : [files]).find { it.name.endsWith('.infer_experiment.txt') }
                                                                                ^^
  ```

- Warning: `workflows/rnaseq/main.nf:548:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .filter { it != null }
                            ^^
  ```

- Warning: `workflows/rnaseq/main.nf:558:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  Channel.value([ [:], ch_biotypes_header_multiqc ]),
                  ^^^^^^^
  ```
