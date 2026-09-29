# Nextflow lint results

- Generated: 2026-09-29T00:26:05.706008+00:00
- Nextflow version: 26.09.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/xengsort/classify/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
