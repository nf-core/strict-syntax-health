# Nextflow lint results

- Generated: 2026-05-27T00:44:25.783294+00:00
- Nextflow version: 26.04.2
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/llamacpppython/run/main.nf:21:5`: Variable was declared but not used

  ```nextflow
      args = task.ext.args ?: ''
      ^^^^^^^^^^
  ```
