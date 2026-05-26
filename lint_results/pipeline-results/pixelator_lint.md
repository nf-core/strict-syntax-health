# Nextflow lint results

- Generated: 2026-05-26T00:39:00.668987170Z
- Nextflow version: 26.04.2
- Summary: 21 warnings

## :warning: Warnings

- Warning: `conf/modules.pna.config:171:89`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_pna_sample_calling_pixelfile || params.save_all ? it : null },
                                                                                          ^^
  ```

- Warning: `conf/modules.pna.config:182:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_json || params.save_all ? it : null },
                                                                  ^^
  ```

- Warning: `subworkflows/local/pna/v1/main.nf:93:5`: Variable was declared but not used

  ```nextflow
      ch_cat_panel_files = ch_cat_fastq
      ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/pna/v1/main.nf:203:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .flatMap { it }
                     ^^
  ```

- Warning: `subworkflows/local/pna/v1/main.nf:207:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def stages = stageFilePairs.collect { it[0] }
                                                    ^^
  ```

- Warning: `subworkflows/local/pna/v1/main.nf:208:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def files = stageFilePairs.collect { it[1] }
                                                   ^^
  ```

- Warning: `subworkflows/local/pna/v2/main.nf:60:5`: Variable was declared but not used

  ```nextflow
      ch_versions = Channel.empty()
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/pna/v2/main.nf:60:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/pna/v2/main.nf:117:5`: Variable was declared but not used

  ```nextflow
      ch_cat_panel_files = ch_cat_fastq
      ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/pna/v2/main.nf:120:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { id, meta, panel_files -> [meta, panel_files] }
                 ^^
  ```

- Warning: `subworkflows/local/pna/v2/main.nf:172:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def parquet = data.collect { it[1] }.flatten()
                                           ^^
  ```

- Warning: `subworkflows/local/pna/v2/main.nf:173:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def reports = data.collect { it[2] }.flatten()
                                           ^^
  ```

- Warning: `subworkflows/local/pna/v2/main.nf:178:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          single: it[1].size() == 1
                  ^^
  ```

- Warning: `subworkflows/local/pna/v2/main.nf:179:16`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          multi: it[1].size() > 1
                 ^^
  ```

- Warning: `subworkflows/local/pna/v2/main.nf:250:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .flatMap { it }
                     ^^
  ```

- Warning: `subworkflows/local/pna/v2/main.nf:254:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def stages = stageFilePairs.collect { it[0] }
                                                    ^^
  ```

- Warning: `subworkflows/local/pna/v2/main.nf:255:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def files = stageFilePairs.collect { it[1] }
                                                   ^^
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

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:76:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/pixelator.nf:109:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions       = ch_versions                 // channel: [ path(versions.yml) ]
      ^^^^^^^^^^^^^^^^^^^^
  ```
