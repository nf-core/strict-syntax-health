# Nextflow lint results

- Generated: 2026-06-22T00:46:01.742512+00:00
- Nextflow version: 26.05.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/humann3/renorm/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
