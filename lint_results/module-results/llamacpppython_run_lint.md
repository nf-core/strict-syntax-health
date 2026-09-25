# Nextflow lint results

- Generated: 2026-09-25T00:25:27.900433+00:00
- Nextflow version: 26.09.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/llamacpppython/run/main.nf:21:5`: Variable was declared but not used

  ```nextflow
      args = task.ext.args ?: ''
      ^^^^^^^^^^
  ```
