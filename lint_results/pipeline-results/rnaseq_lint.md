# Nextflow lint results

- Generated: 2026-04-01T00:30:07.832281023Z
- Nextflow version: 26.03.1-edge
- Summary: 7 warnings

## :warning: Warnings

- Warning: `subworkflows/local/prepare_genome/main.nf:194:79`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_transcript_fasta = GFFREAD_TRANSCRIPTS.out.gffread_fasta.map { meta, fasta_file -> fasta_file }
                                                                                ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:390:120`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ch_bowtie2_index = UNTAR_BOWTIE2_INDEX ([ [:], file(bowtie2_index, checkIfExists: true) ]).untar.map { meta, index -> index }
                                                                                                                         ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:400:62`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_bowtie2_index = BOWTIE2_BUILD.out.index.map { meta, index -> index }
                                                               ^^^^
  ```

- Warning: `subworkflows/nf-core/quant_tximport_summarizedexperiment/main.nf:33:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, results -> [ [:], results ] }
                 ^^^^
  ```

- Warning: `workflows/rnaseq/main.nf:534:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, bam, gtf, biotype_ok -> biotype_ok }
                        ^^^^
  ```

- Warning: `workflows/rnaseq/main.nf:534:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, bam, gtf, biotype_ok -> biotype_ok }
                              ^^^
  ```

- Warning: `workflows/rnaseq/main.nf:534:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, bam, gtf, biotype_ok -> biotype_ok }
                                   ^^^
  ```
