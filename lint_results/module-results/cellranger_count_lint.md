# Nextflow lint results

- Generated: 2026-02-13T00:24:57.180906+00:00
- Nextflow version: 26.01.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/cellranger/count/main.nf:23:5`: Variable was declared but not used

  ```nextflow
      args = task.ext.args ?: ''
      ^^^^^^^^^^
  ```
