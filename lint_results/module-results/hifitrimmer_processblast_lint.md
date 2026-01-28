# Nextflow lint results

- Generated: 2026-01-28T00:19:42.724495+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/hifitrimmer/processblast/main.nf:25:8`: Variable was declared but not used

  ```nextflow
     def prefix = task.ext.prefix ?: "${meta.id}"
         ^^^^^^^^^^
  ```
