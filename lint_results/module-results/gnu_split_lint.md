# Nextflow lint results

- Generated: 2026-01-23T00:22:21.958961+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/gnu/split/main.nf:47:9`: Variable was declared but not used

  ```nextflow
      def args        = task.ext.args   ?: ''
          ^^^^^^^^^^
  ```
