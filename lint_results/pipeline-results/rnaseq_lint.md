# Nextflow lint results

- Generated: 2026-03-25T00:27:25.086242470Z
- Nextflow version: 26.03.0-edge
- Summary: 7 warnings

## :warning: Warnings

- Warning: `subworkflows/local/prepare_genome/main.nf:191:79`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_transcript_fasta = GFFREAD_TRANSCRIPTS.out.gffread_fasta.map { meta, fasta_file -> fasta_file }
                                                                                ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:387:120`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ch_bowtie2_index = UNTAR_BOWTIE2_INDEX ([ [:], file(bowtie2_index, checkIfExists: true) ]).untar.map { meta, index -> index }
                                                                                                                         ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:397:62`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_bowtie2_index = BOWTIE2_BUILD.out.index.map { meta, index -> index }
                                                               ^^^^
  ```

- Warning: `subworkflows/nf-core/quant_tximport_summarizedexperiment/main.nf:33:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, results -> [ [:], results ] }
                 ^^^^
  ```

- Warning: `workflows/rnaseq/main.nf:533:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, bam, gtf, biotype_ok -> biotype_ok }
                        ^^^^
  ```

- Warning: `workflows/rnaseq/main.nf:533:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, bam, gtf, biotype_ok -> biotype_ok }
                              ^^^
  ```

- Warning: `workflows/rnaseq/main.nf:533:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, bam, gtf, biotype_ok -> biotype_ok }
                                   ^^^
  ```
