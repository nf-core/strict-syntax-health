# Nextflow lint results

- Generated: 2026-07-04T00:37:31.202920+00:00
- Nextflow version: 26.06.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/llamacpppython/run/main.nf:21:5`: Variable was declared but not used

  ```nextflow
      args = task.ext.args ?: ''
      ^^^^^^^^^^
  ```
