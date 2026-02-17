# Nextflow lint results

- Generated: 2026-02-17T00:24:27.778319+00:00
- Nextflow version: 26.01.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/purecn/normaldb/main.nf:29:9`: Variable was declared but not used

  ```nextflow
      def prefix          = task.ext.prefix   ?: "${meta.id}"
          ^^^^^^^^^^
  ```
