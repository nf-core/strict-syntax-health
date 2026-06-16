# Nextflow lint results

- Generated: 2026-06-16T14:27:47.273692606Z
- Nextflow version: 26.04.3
- Summary: 5 warnings

## :warning: Warnings

- Warning: `main.nf:65:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = PROTEINANNOTATOR.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/functional_annotation/main.nf:31:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      interproscan_tsv = ch_interproscan_tsv
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
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

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:76:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```
