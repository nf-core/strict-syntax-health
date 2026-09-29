# Nextflow lint results

- Generated: 2026-09-29T00:21:18.086139834Z
- Nextflow version: 26.09.1-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `subworkflows/local/utils_nfcore_datasync_pipeline/main.nf:200:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def requires_download = samples.any { meta, input_path, output_path, md5, sha ->
                                            ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_datasync_pipeline/main.nf:200:61`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def requires_download = samples.any { meta, input_path, output_path, md5, sha ->
                                                              ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_datasync_pipeline/main.nf:200:74`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def requires_download = samples.any { meta, input_path, output_path, md5, sha ->
                                                                           ^^^
  ```
