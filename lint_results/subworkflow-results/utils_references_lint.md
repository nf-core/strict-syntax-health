# Nextflow lint results

- Generated: 2026-04-10T00:29:01.289259+00:00
- Nextflow version: 26.03.2-edge
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
