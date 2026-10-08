# Nextflow lint results

- Generated: 2026-10-08T00:30:58.868333829Z
- Nextflow version: 26.09.2-edge
- Summary: 10 warnings

## :warning: Warnings

- Warning: `modules/local/experiment_summary/main.nf:30:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def stageArray = result_stages.collect { "\"${it}\"" }.join(' ')
                                                    ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pixelator_pipeline/main.nf:279:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .flatMap { it }
                     ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pixelator_pipeline/main.nf:290:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              tuple([id: 'all'], filtered.collect { it[0] }, filtered.collect { it[1] })
                                                    ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pixelator_pipeline/main.nf:290:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              tuple([id: 'all'], filtered.collect { it[0] }, filtered.collect { it[1] })
                                                                                ^^
  ```

- Warning: `workflows/proxiome_v1.nf:79:5`: Variable was declared but not used

  ```nextflow
      ch_checked_panel_files = ch_panel_files
      ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/proxiome_v2.nf:106:5`: Variable was declared but not used

  ```nextflow
      ch_checked_panel_files = ch_panel_files_grouped_by_pool
      ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/proxiome_v2.nf:170:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def parquet = data.collect { it[1] }.flatten()
                                           ^^
  ```

- Warning: `workflows/proxiome_v2.nf:171:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def reports = data.collect { it[2] }.flatten()
                                           ^^
  ```

- Warning: `workflows/proxiome_v2.nf:176:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          single: it[1].size() == 1
                  ^^
  ```

- Warning: `workflows/proxiome_v2.nf:177:16`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          multi: it[1].size() > 1
                 ^^
  ```
