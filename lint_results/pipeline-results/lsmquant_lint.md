# Nextflow lint results

- Generated: 2026-03-21T00:23:23.404799177Z
- Nextflow version: 26.03.0-edge
- Summary: 1 error, 38 warnings

## :x: Errors

- Error: `workflows/lsmquant.nf:137:26`: `img_dir` is already declared

  ```nextflow
              .map { meta, img_dir, parameter_file, stitched_data ->
                           ^^^^^^^
  ```

## :warning: Warnings

- Warning: `modules/local/mat2json/main.nf:20:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/mat2json/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/numorph3dunet/main.nf:45:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/numorphalign/main.nf:25:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/numorphalign/main.nf:48:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/numorphregister/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/numorphregister/main.nf:48:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/numorphstitch/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/numorphstitch/main.nf:50:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/stagefiles/main.nf:20:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/stagefiles/main.nf:41:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/stagefiles/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/mat2json/main.nf:19:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/mat2json/main.nf:37:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/numorph/intensity/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/numorph/intensity/main.nf:39:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/unzip/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/araregistration/main.nf:14:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/araregistration/main.nf:15:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      sample_meta = stitched_data.map { meta, img_dir, params -> meta }
                                              ^^^^^^^
  ```

- Warning: `subworkflows/local/araregistration/main.nf:15:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      sample_meta = stitched_data.map { meta, img_dir, params -> meta }
                                                       ^^^^^^
  ```

- Warning: `subworkflows/local/araregistration/main.nf:21:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, stitched_img_directory, parameter_file, resampled ->
                       ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/numorph_preprocessing/main.nf:33:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .findAll { it.name.endsWith('.mat') }
                             ^^
  ```

- Warning: `subworkflows/local/numorph_stitch/main.nf:28:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .findAll { it.name.endsWith('.mat') }
                             ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_lsmquant_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_lsmquant_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_lsmquant_pipeline/main.nf:103:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_samplesheet = Channel.fromList(samplesheetToList(params.input, "${projectDir}/assets/schema_input.json"))
                       ^^^^^^^
  ```

- Warning: `workflows/lsmquant.nf:36:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `workflows/lsmquant.nf:37:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/lsmquant.nf:41:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_parameter_file = samplesheet.map { meta, img_dir, parameter_file -> [meta, parameter_file] }
                                                  ^^^^^^^
  ```

- Warning: `workflows/lsmquant.nf:57:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, zip, parameter_file ->
                            ^^^^^^^^^^^^^^
  ```

- Warning: `workflows/lsmquant.nf:67:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, unzipped, zip, parameter_file ->
                                 ^^^
  ```

- Warning: `workflows/lsmquant.nf:74:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, img_directory, parameter_file ->
                                      ^^^^^^^^^^^^^^
  ```

- Warning: `workflows/lsmquant.nf:84:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, staged, raw_img_directory, parameter_file ->
                               ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/lsmquant.nf:90:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_samplesheet = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `workflows/lsmquant.nf:111:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .findAll { it.name.endsWith('.mat') }
                             ^^
  ```

- Warning: `workflows/lsmquant.nf:137:26`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, img_dir, parameter_file, stitched_data ->
                           ^^^^^^^
  ```

- Warning: `workflows/lsmquant.nf:144:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          def model_file = Channel.fromPath(params.model_file, checkIfExists: !params.model_file.startsWith('http'))
                           ^^^^^^^
  ```

- Warning: `workflows/lsmquant.nf:158:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```
