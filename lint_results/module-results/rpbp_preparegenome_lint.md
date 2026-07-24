# Nextflow lint results

- Generated: 2026-07-24T00:30:42.262494+00:00
- Nextflow version: 26.07.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/rpbp/preparegenome/main.nf:23:5`: Variable was declared but not used

  ```nextflow
      task_ext_args = task.ext.args ?: ''
      ^^^^^^^^^^
  ```
