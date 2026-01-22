# Nextflow lint results

- Generated: 2026-01-22T00:21:30.773417+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/rundbcan/easysubstrate/main.nf:69:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
