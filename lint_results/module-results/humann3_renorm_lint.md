# Nextflow lint results

- Generated: 2026-08-07T01:18:22.102030+00:00
- Nextflow version: 26.07.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/humann3/renorm/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
