# Nextflow lint results

- Generated: 2026-06-24T00:35:25.037450490Z
- Nextflow version: 26.05.0-edge
- Summary: 5 warnings

## :warning: Warnings

- Warning: `main.nf:61:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = DATASYNC.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
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

- Warning: `workflows/datasync.nf:40:5`: Variable was declared but not used

  ```nextflow
      ch_checksum = ch_samplesheet.checksum.branch {
      ^^^^^^^^^^^
  ```
