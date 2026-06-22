# Nextflow lint results

- Generated: 2026-06-22T00:46:01.756159+00:00
- Nextflow version: 26.05.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/llamacpppython/run/main.nf:21:5`: Variable was declared but not used

  ```nextflow
      args = task.ext.args ?: ''
      ^^^^^^^^^^
  ```
