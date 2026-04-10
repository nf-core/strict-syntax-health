# Nextflow lint results

- Generated: 2026-04-10T00:26:01.689921851Z
- Nextflow version: 26.03.2-edge
- Summary: 10 warnings

## :warning: Warnings

- Warning: `subworkflows/local/bam_post_alignment_qc/main.nf:55:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, bam, gtf, biotype_ok -> biotype_ok }
                        ^^^^
  ```

- Warning: `subworkflows/local/bam_post_alignment_qc/main.nf:55:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, bam, gtf, biotype_ok -> biotype_ok }
                              ^^^
  ```

- Warning: `subworkflows/local/bam_post_alignment_qc/main.nf:55:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, bam, gtf, biotype_ok -> biotype_ok }
                                   ^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:193:79`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_transcript_fasta = GFFREAD_TRANSCRIPTS.out.gffread_fasta.map { meta, fasta_file -> fasta_file }
                                                                                ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:379:120`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ch_bowtie2_index = UNTAR_BOWTIE2_INDEX ([ [:], file(bowtie2_index, checkIfExists: true) ]).untar.map { meta, index -> index }
                                                                                                                         ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:389:62`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_bowtie2_index = BOWTIE2_BUILD.out.index.map { meta, index -> index }
                                                               ^^^^
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

- Warning: `workflows/rnaseq/main.nf:541:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      def ie = (files instanceof List ? files : [files]).find { it.name.endsWith('.infer_experiment.txt') }
                                                                                ^^
  ```

- Warning: `workflows/rnaseq/main.nf:544:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .filter { it != null }
                            ^^
  ```
