# Nextflow lint results

- Generated: 2026-07-07T00:37:20.897607482Z
- Nextflow version: 26.06.0-edge
- Summary: 4 warnings

## :warning: Warnings

- Warning: `subworkflows/local/utils_nfcore_references_pipeline/main.nf:168:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      references = references
      ^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_references/main.nf:28:5`: Variable was declared but not used

  ```nextflow
      references_file = get_references_file(references, param_file, attribute_file)
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_references/main.nf:29:5`: Variable was declared but not used

  ```nextflow
      references_value = get_references_value(references, param_value, attribute_value)
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/references.nf:101:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      references = references // channel: [meta, *]
      ^^^^^^^^^^^^^^^^^^^^^
  ```
