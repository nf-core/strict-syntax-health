# Nextflow lint results

- Generated: 2026-07-07T00:37:37.405831776Z
- Nextflow version: 26.06.0-edge
- Summary: 13 warnings

## :warning: Warnings

- Warning: `modules/nf-core/cat/cat/main.nf:23:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def file_list = files_in.collect { it.toString() }
                                         ^^
  ```

- Warning: `modules/nf-core/cat/cat/main.nf:58:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def file_list   = files_in.collect { it.toString() }
                                           ^^
  ```

- Warning: `subworkflows/local/merge_ids/main.nf:37:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, file, count -> [ meta, file ] }
                                 ^^^^^
  ```

- Warning: `subworkflows/local/merge_ids/main.nf:46:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, file, count -> [ meta, file ] }
                                 ^^^^^
  ```

- Warning: `subworkflows/local/report/main.nf:7:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      use_centroid
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/report/main.nf:8:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      min_score
      ^^^^^^^^^
  ```

- Warning: `subworkflows/local/report/main.nf:22:5`: Variable was declared but not used

  ```nextflow
      ch_fasta     = ch_seqinfo.map { row -> [row[0], []] }
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/score_orthologs/main.nf:29:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { id, score, query, taxid, exact -> [id, score, query] }
                                   ^^^^^
  ```

- Warning: `subworkflows/local/score_orthologs/main.nf:29:41`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { id, score, query, taxid, exact -> [id, score, query] }
                                          ^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nextflow_pipeline/main.nf:43:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:20:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      valid_config = valid_config
      ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:72:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/reportho.nf:96:5`: Variable was declared but not used

  ```nextflow
      ch_samplesheet = ch_samplesheet_query.mix (ch_samplesheet_fasta)
      ^^^^^^^^^^^^^^
  ```
