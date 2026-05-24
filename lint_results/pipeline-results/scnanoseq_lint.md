# Nextflow lint results

- Generated: 2026-05-24T00:37:56.519055637Z
- Nextflow version: 26.04.2
- Summary: 1 error, 5 warnings

## :x: Errors

- Error: `workflows/scnanoseq.nf:555:65`: `ch_versions_yaml` is not defined

  ```nextflow
              ch_multiqc_rawqc_files = ch_multiqc_rawqc_files.mix(ch_versions_yaml.collect())
                                                                  ^^^^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `main.nf:45:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = SCNANOSEQ.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
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
