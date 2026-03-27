# Nextflow lint results

- Generated: 2026-03-27T00:27:27.425626+00:00
- Nextflow version: 26.03.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/custom/geneticmapconvert/main.nf:25:5`: Variable was declared but not used

  ```nextflow
      args = task.ext.args ?: ''
      ^^^^^^^^^^
  ```
