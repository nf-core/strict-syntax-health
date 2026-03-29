# Nextflow lint results

- Generated: 2026-03-29T00:25:45.630951+00:00
- Nextflow version: 26.03.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/custom/geneticmapconvert/main.nf:25:5`: Variable was declared but not used

  ```nextflow
      args = task.ext.args ?: ''
      ^^^^^^^^^^
  ```
