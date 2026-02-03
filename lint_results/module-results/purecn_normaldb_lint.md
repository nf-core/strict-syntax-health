# Nextflow lint results

- Generated: 2026-02-03T00:25:25.910625+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/purecn/normaldb/main.nf:29:9`: Variable was declared but not used

  ```nextflow
      def prefix          = task.ext.prefix   ?: "${meta.id}"
          ^^^^^^^^^^
  ```
