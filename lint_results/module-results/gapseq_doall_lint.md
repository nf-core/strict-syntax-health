# Nextflow lint results

- Generated: 2026-06-22T00:46:01.715045+00:00
- Nextflow version: 26.05.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/gapseq/doall/main.nf:26:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^^^^^
  ```
