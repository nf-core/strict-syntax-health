# Nextflow lint results

- Generated: 2026-08-07T01:18:22.071791+00:00
- Nextflow version: 26.07.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/gapseq/doall/main.nf:27:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^^^^^
  ```
