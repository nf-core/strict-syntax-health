# Nextflow lint results

- Generated: 2026-06-16T20:18:26.176256878Z
- Nextflow version: 26.04.3
- Summary: 2 errors, 14 warnings

## :x: Errors

- Error: `workflows/cellpainting.nf:104:33`: `sortGroupedImages` is not defined

  ```nextflow
              def (m, im, imgs) = sortGroupedImages(meta, images_meta, images)
                                  ^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/cellpainting.nf:199:37`: `sortGroupedImages` is not defined

  ```nextflow
                  def (m, im, imgs) = sortGroupedImages(meta, images_meta, images)
                                      ^^^^^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `main.nf:50:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = CELLPAINTING.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_cellpainting_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_cellpainting_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_cellpainting_pipeline/main.nf:99:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nextflow_pipeline/main.nf:43:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:20:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      valid_config
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:72:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/cellpainting.nf:43:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          [meta, sorted.collect { it[0] }, sorted.collect { it[1] }]
                                  ^^
  ```

- Warning: `workflows/cellpainting.nf:43:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          [meta, sorted.collect { it[0] }, sorted.collect { it[1] }]
                                                            ^^
  ```

- Warning: `workflows/cellpainting.nf:155:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              [plate_key, plate_meta, sorted.collect { it[0] }, sorted.collect { it[1] }]
                                                       ^^
  ```

- Warning: `workflows/cellpainting.nf:155:80`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              [plate_key, plate_meta, sorted.collect { it[0] }, sorted.collect { it[1] }]
                                                                                 ^^
  ```

- Warning: `workflows/cellpainting.nf:230:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .collect { it[1] }
                                 ^^
  ```

- Warning: `workflows/cellpainting.nf:242:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```
