# Nextflow lint results

- Generated: 2026-06-04T00:49:33.797298005Z
- Nextflow version: 26.04.3
- Summary: 5 warnings

## :warning: Warnings

- Warning: `conf/modules/mutect2.config:50:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { meta.num_intervals > 1 ? null : it },
                                                        ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_createpanelrefs_pipeline/main.nf:124:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      samplesheet = ch_samplesheet
      ^^^^^^^^^^^^^^^^^^^^^^^^^^
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
