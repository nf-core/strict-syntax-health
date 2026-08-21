# Nextflow lint results

- Generated: 2026-08-21T00:15:22.087168+00:00
- Nextflow version: 26.08.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/misopy/index/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^^^^^
  ```
