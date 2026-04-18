# Nextflow lint results

- Generated: 2026-04-18T00:28:51.731320297Z
- Nextflow version: 26.03.2-edge
- Summary: 3 warnings

## :warning: Warnings

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

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```
