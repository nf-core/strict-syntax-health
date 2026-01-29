# Nextflow lint results

- Generated: 2026-01-29T00:22:49.027671+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/tcoffee/irmsd/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
