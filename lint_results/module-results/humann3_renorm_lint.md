# Nextflow lint results

- Generated: 2026-09-25T00:25:27.882503+00:00
- Nextflow version: 26.09.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/humann3/renorm/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
