# Nextflow lint results

- Generated: 2026-02-12T00:24:23.112259+00:00
- Nextflow version: 26.01.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/cellbender/merge/main.nf:22:5`: Variable was declared but not used

  ```nextflow
      output_layer = task.ext.output_layer ?: "cellbender"
      ^^^^^^^^^^
  ```
