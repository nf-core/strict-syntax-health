# Nextflow lint results

- Generated: 2026-04-29T00:35:22.772779592Z
- Nextflow version: 26.03.4-edge
- Summary: 2 errors, 7 warnings

## :x: Errors

- Error: `workflows/cellpainting.nf:102:33`: `sortGroupedImages` is not defined

  ```nextflow
              def (m, im, imgs) = sortGroupedImages(meta, images_meta, images)
                                  ^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/cellpainting.nf:133:37`: `sortGroupedImages` is not defined

  ```nextflow
                  def (m, im, imgs) = sortGroupedImages(meta, images_meta, images)
                                      ^^^^^^^^^^^^^^^^^
  ```

## :warning: Warnings

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

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```

- Warning: `workflows/cellpainting.nf:41:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          [meta, sorted.collect { it[0] }, sorted.collect { it[1] }]
                                  ^^
  ```

- Warning: `workflows/cellpainting.nf:41:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          [meta, sorted.collect { it[0] }, sorted.collect { it[1] }]
                                                            ^^
  ```

- Warning: `workflows/cellpainting.nf:162:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```
