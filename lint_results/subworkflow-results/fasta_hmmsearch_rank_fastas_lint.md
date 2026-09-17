# Nextflow lint results

- Generated: 2026-09-17T00:25:12.938632+00:00
- Nextflow version: 26.08.0-edge
- Summary: 7 warnings

## :warning: Warnings

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:33:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { pairs -> [ [ id: 'rank.tblout' ], pairs.collect { it[0] }, pairs.collect { it[1] } ] }
                                                                   ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:33:91`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { pairs -> [ [ id: 'rank.tblout' ], pairs.collect { it[0] }, pairs.collect { it[1] } ] }
                                                                                            ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:48:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { pairs -> [ [ id: 'rank.domtblout' ], pairs.collect { it[0] }, pairs.collect { it[1] } ] }
                                                                          ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:48:98`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { pairs -> [ [ id: 'rank.domtblout' ], pairs.collect { it[0] }, pairs.collect { it[1] } ] }
                                                                                                   ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:54:81`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_domtblout_parquet = DUCKDB_TABLE2PARQUET_DOMTBLOUT.out.parquet.map { meta, parquet -> parquet }
                                                                                  ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:56:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_domtblout_parquet = Channel.value([])
                                 ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:63:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, parquet -> [ [ id: 'rank' ], parquet ] }
                 ^^^^^^^^^^
  ```
