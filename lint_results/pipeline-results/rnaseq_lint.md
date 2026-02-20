# Nextflow lint results

- Generated: 2026-02-20T00:21:28.857484589Z
- Nextflow version: 26.01.1-edge
- Summary: 5 warnings

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

- Warning: `subworkflows/local/prepare_genome/main.nf:398:62`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_bowtie2_index = BOWTIE2_BUILD.out.index.map { meta, index -> index }
                                                               ^^^^
  ```

- Warning: `subworkflows/nf-core/quantify_rsem/main.nf:46:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_counts_gene.collect{ it[1] }.map { results -> [ ['id': 'all_samples'], results ] },
                                  ^^
  ```

- Warning: `subworkflows/nf-core/quantify_rsem/main.nf:47:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_counts_transcript.collect{ it[1] }
                                        ^^
  ```
