# Nextflow lint results

- Generated: 2026-09-25T00:25:27.843971+00:00
- Nextflow version: 26.09.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/gapseq/findtransport/main.nf:24:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^^^^^
  ```
