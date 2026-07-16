# Nextflow lint results

- Generated: 2026-07-16T00:29:17.746973703Z
- Nextflow version: 26.06.0-edge
- Summary: 7 warnings

## :warning: Warnings

- Warning: `main.nf:620:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = ch_multiqc
      ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/boltz_fasta/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/run_helixfold3/main.nf:114:9`: Variable was declared but not used

  ```nextflow
      def VERSION = '705c2974a833cdc3a4420f4e3379da596091c97f'
          ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_proteinfold_pipeline/main.nf:327:78`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def unsupportedModes = requestedModes.findAll { !supportedModes.contains(it) }.unique().sort()
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

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:72:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```
