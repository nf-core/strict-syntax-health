# Nextflow lint results

- Generated: 2026-05-19T00:40:32.845503297Z
- Nextflow version: 26.04.1
- Summary: 15 warnings

## :warning: Warnings

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
