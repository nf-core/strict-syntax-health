# Nextflow lint results

- Generated: 2026-07-28T00:36:56.738137+00:00
- Nextflow version: 26.07.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/eigenstratdatabasetools/eigenstratsnpcoverage/main.nf:35:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
