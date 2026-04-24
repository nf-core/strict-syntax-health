# Nextflow lint results

- Generated: 2026-04-24T00:34:05.873681+00:00
- Nextflow version: 26.03.3-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/nf-core/utils_references/main.nf:24:5`: Variable was declared but not used

  ```nextflow
      references_file = get_references_file(references, param_file, attribute_file, basepath)
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_references/main.nf:25:5`: Variable was declared but not used

  ```nextflow
      references_value = get_references_value(references, param_value, attribute_value)
      ^^^^^^^^^^
  ```
