# Nextflow lint results

- Generated: 2026-08-13T00:25:18.906278+00:00
- Nextflow version: 26.07.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/llamacpppython/run/main.nf:21:5`: Variable was declared but not used

  ```nextflow
      args = task.ext.args ?: ''
      ^^^^^^^^^^
  ```
