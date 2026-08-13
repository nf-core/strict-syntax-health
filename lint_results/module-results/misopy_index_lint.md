# Nextflow lint results

- Generated: 2026-08-13T00:25:18.919579+00:00
- Nextflow version: 26.07.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/misopy/index/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^^^^^
  ```
