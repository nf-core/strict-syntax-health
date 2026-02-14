# Nextflow lint results

- Generated: 2026-02-14T00:20:18.559686311Z
- Nextflow version: 26.01.1-edge
- Summary: 49 warnings

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

- Warning: `modules/local/numorph3dunet/main.nf:52:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/numorphalign/main.nf:29:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/numorphalign/main.nf:30:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/numorphalign/main.nf:56:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/numorphalign/main.nf:57:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/numorphintensity/main.nf:24:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/numorphintensity/main.nf:25:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/numorphintensity/main.nf:46:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/numorphintensity/main.nf:47:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
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

- Warning: `modules/local/numorphresample/main.nf:18:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/numorphresample/main.nf:19:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/numorphresample/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/numorphstitch/main.nf:26:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/numorphstitch/main.nf:27:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/numorphstitch/main.nf:75:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/numorphstitch/main.nf:76:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
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

- Warning: `subworkflows/local/araregistration/main.nf:26:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, resampled, stitched_img_directory, parameter_file ->
                                  ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/numorph_preprocessing/main.nf:17:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/numorph_preprocessing/main.nf:19:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      sample_meta = samplesheet.map { meta, img_dir, params -> meta }
                                            ^^^^^^^
  ```

- Warning: `subworkflows/local/numorph_preprocessing/main.nf:19:52`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      sample_meta = samplesheet.map { meta, img_dir, params -> meta }
                                                     ^^^^^^
  ```

- Warning: `subworkflows/local/numorph_stitch/main.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/numorph_stitch/main.nf:18:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      sample_meta = samplesheet.map { meta, img_dir, params -> meta }
                                            ^^^^^^^
  ```

- Warning: `subworkflows/local/numorph_stitch/main.nf:18:52`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      sample_meta = samplesheet.map { meta, img_dir, params -> meta }
                                                     ^^^^^^
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

- Warning: `workflows/lsmquant.nf:36:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/lsmquant.nf:37:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `workflows/lsmquant.nf:51:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, zip, parameter_file ->
                            ^^^^^^^^^^^^^^
  ```

- Warning: `workflows/lsmquant.nf:62:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, unzipped, zip, parameter_file ->
                                 ^^^
  ```

- Warning: `workflows/lsmquant.nf:69:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, img_directory, parameter_file ->
                                      ^^^^^^^^^^^^^^
  ```

- Warning: `workflows/lsmquant.nf:80:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, staged, raw_img_directory, parameter_file ->
                               ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/lsmquant.nf:86:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_samplesheet = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `workflows/lsmquant.nf:115:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, stitched, raw_img_directory, parameter_file ->
                                     ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/lsmquant.nf:130:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, stitched, raw_img_directory, parameter_file ->
                                     ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/lsmquant.nf:145:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, stitched, raw_img_directory, parameter_file ->
                                     ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/lsmquant.nf:153:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          model_file = Channel.fromPath(params.model_file, checkIfExists: !params.model_file.startsWith('http'))
                       ^^^^^^^
  ```

- Warning: `workflows/lsmquant.nf:166:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```
