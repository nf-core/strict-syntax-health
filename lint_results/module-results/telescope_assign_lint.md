# Nextflow lint results

- Generated: 2026-04-09T00:24:16.101111+00:00
- Nextflow version: 26.03.2-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/telescope/assign/main.nf:26:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta_bam.id}"
          ^^^^^^^^^^
  ```
