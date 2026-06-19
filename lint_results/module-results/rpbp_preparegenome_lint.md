# Nextflow lint results

- Generated: 2026-06-19T00:54:55.658960+00:00
- Nextflow version: 26.04.4
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/rpbp/preparegenome/main.nf:23:5`: Variable was declared but not used

  ```nextflow
      task_ext_args = task.ext.args ?: ''
      ^^^^^^^^^^
  ```
