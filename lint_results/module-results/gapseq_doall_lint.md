# Nextflow lint results

- Generated: 2026-06-15T00:46:05.155728+00:00
- Nextflow version: 26.04.3
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/gapseq/doall/main.nf:26:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^^^^^
  ```
