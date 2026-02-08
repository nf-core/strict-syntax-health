# Nextflow lint results

- Generated: 2026-02-08T00:29:10.307470+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/kat/hist/main.nf:59:9`: Variable was declared but not used

  ```nextflow
      def args      = task.ext.args   ?: ''
          ^^^^^^^^^^
  ```
