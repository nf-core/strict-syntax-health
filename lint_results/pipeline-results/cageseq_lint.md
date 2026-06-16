# Nextflow lint results

- Generated: 2026-06-16T20:18:04.144790878Z
- Nextflow version: 26.04.3
- Summary: 6 warnings

## :warning: Warnings

- Warning: `main.nf:58:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = CAGESEQ.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/input_from_folder/main.nf:54:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      ch_fastq = ch_fastq
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/mapped_inputs/main.nf:15:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      input_files = input_files
      ^^^^^^^^^^^^^^^^^^^^^^^
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
