# Nextflow lint results

- Generated: 2026-11-19T00:15:01.399982237Z
- Nextflow version: 26.11.0-edge
- Summary: 12 warnings

## :warning: Warnings

- Warning: `modules/local/experiment_summary/main.nf:31:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def stageArray = result_stages.collect { "\"${it}\"" }.join(' ')
                                                    ^^
  ```

- Warning: `modules/local/pixelator/aggregate/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pixelator/analysis/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pixelator/denoise/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pixelator/edgelist/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pixelator/graph/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pixelator/graph_collapse/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pixelator/list_options/main.nf:14:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pixelator/sample_calling/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pixelator_pipeline/main.nf:261:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .flatMap { it }
                     ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pixelator_pipeline/main.nf:272:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              tuple([id: 'all'], filtered.collect { it[0] }, filtered.collect { it[1] })
                                                    ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pixelator_pipeline/main.nf:272:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              tuple([id: 'all'], filtered.collect { it[0] }, filtered.collect { it[1] })
                                                                                ^^
  ```
