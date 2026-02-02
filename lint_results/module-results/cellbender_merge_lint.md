# Nextflow lint results

- Generated: 2026-02-02T00:19:53.335304+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/cellbender/merge/main.nf:22:5`: Variable was declared but not used

  ```nextflow
      output_layer = task.ext.output_layer ?: "cellbender"
      ^^^^^^^^^^
  ```
