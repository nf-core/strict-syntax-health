# Nextflow lint results

- Generated: 2026-06-15T00:46:05.235670+00:00
- Nextflow version: 26.04.3
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/rpbp/preparegenome/main.nf:23:5`: Variable was declared but not used

  ```nextflow
      task_ext_args = task.ext.args ?: ''
      ^^^^^^^^^^
  ```
