# Nextflow lint results

- Generated: 2026-10-09T00:26:15.311557374Z
- Nextflow version: 26.09.2-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/local/ldak/calcinflation/main.nf:21:5`: Variable was declared but not used

  ```nextflow
      quarter_reml_files_r = quarter_reml_files.sort { a, b -> a.name <=> b.name }.collect { quarterFile -> "\"${quarterFile}\"" }.join(', ')
      ^^^^^^^^^^^^^^^^^^^^
  ```
