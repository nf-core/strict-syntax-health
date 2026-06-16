# Nextflow lint results

- Generated: 2026-06-16T14:29:03.647913820Z
- Nextflow version: 26.04.3
- Summary: 5 warnings

## :warning: Warnings

- Warning: `subworkflows/local/utils_nfcore_rangeland_pipeline/main.nf:102:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions    = ch_versions
      ^^^^^^^^^^^^^^^^^^^^
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

- Warning: `workflows/rangeland.nf:166:5`: Variable was declared but not used

  ```nextflow
      grouped_trend_data = HIGHER_LEVEL.out.mosaic.map{ it -> it[1] }.flatten().buffer( size: Integer.MAX_VALUE, remainder: true )
      ^^^^^^^^^^^^^^^^^^
  ```
