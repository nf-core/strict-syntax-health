# Nextflow lint results

- Generated: 2026-02-13T00:24:57.261570+00:00
- Nextflow version: 26.01.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/opt/track/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
