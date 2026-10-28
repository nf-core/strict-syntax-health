# Nextflow lint results

- Generated: 2026-10-28T00:17:02.302490258Z
- Nextflow version: 26.10.4
- Summary: 29 warnings

## :warning: Warnings

- Warning: `modules/local/hmmer/hmmextract/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/clustalo/align/main.nf:24:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/custom/resolvetaxonomy/main.nf:28:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/duckdb/table2parquet/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/epang/place/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/epang/split/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gappa/editmerge/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gappa/examineassign/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gappa/examinegraft/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gappa/examineheattree/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/hmmer/eslalimask/main.nf:25:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/hmmer/eslreformat/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/hmmer/formattsv/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/hmmer/hmmalign/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/hmmer/hmmbuild/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/hmmer/hmmrank/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/hmmer/hmmsearch/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/mafft/align/main.nf:24:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/multiqc/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/seqtk/subseq/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:35:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { pairs -> pairs.sort { it[0] } }
                                       ^^
  ```

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:36:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { pairs -> [ [ id: 'rank.tblout' ], pairs.collect { it[0] }, pairs.collect { it[1] } ] }
                                                                   ^^
  ```

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:36:91`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { pairs -> [ [ id: 'rank.tblout' ], pairs.collect { it[0] }, pairs.collect { it[1] } ] }
                                                                                            ^^
  ```

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:52:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { pairs -> pairs.sort { it[0] } }
                                           ^^
  ```

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:53:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { pairs -> [ [ id: 'rank.domtblout' ], pairs.collect { it[0] }, pairs.collect { it[1] } ] }
                                                                          ^^
  ```

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:53:98`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { pairs -> [ [ id: 'rank.domtblout' ], pairs.collect { it[0] }, pairs.collect { it[1] } ] }
                                                                                                   ^^
  ```

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:59:81`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_domtblout_parquet = DUCKDB_TABLE2PARQUET_DOMTBLOUT.out.parquet.map { meta, parquet -> parquet }
                                                                                  ^^^^
  ```

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:61:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_domtblout_parquet = Channel.value([])
                                 ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:68:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, parquet -> [ [ id: 'rank' ], parquet ] }
                 ^^^^
  ```
