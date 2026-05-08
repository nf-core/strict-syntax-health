# Nextflow lint results

- Generated: 2026-05-08T00:35:03.515309341Z
- Nextflow version: 26.04.0
- Summary: 2 warnings

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
