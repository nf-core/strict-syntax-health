# Nextflow lint results

- Generated: 2026-03-06T00:27:04.195818+00:00
- Nextflow version: 26.02.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/purgedups/purgedups/main.nf:24:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^^^^^
  ```
