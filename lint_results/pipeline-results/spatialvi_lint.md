# Nextflow lint results

- Generated: 2026-06-16T20:42:48.503438053Z
- Nextflow version: 26.04.3
- Summary: 8 warnings

## :warning: Warnings

- Warning: `main.nf:108:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = SPATIALVI.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/clustering/main.nf:50:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      adata = SCANPY_LEIDEN.out.adata // channel: [ meta, h5ad ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/input_check/main.nf:40:5`: Variable was declared but not used

  ```nextflow
      ch_spaceranger_input = ch_spaceranger_combined
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/input_check/main.nf:62:5`: Variable was declared but not used

  ```nextflow
      ch_downstream_input = ch_downstream_combined
      ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/spaceranger/main.nf:52:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      sr_dir = SPACERANGER_COUNT.out.outs // channel: [ meta, dir ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
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
