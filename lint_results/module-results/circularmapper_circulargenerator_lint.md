# Nextflow lint results

- Generated: 2026-02-02T00:19:53.344767+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/circularmapper/circulargenerator/main.nf:50:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
