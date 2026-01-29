# Nextflow lint results

- Generated: 2026-01-29T00:22:48.887844+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/chewbbaca/allelecall/main.nf:62:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
