# Nextflow lint results

- Generated: 2026-08-06T00:30:54.996505+00:00
- Nextflow version: 26.07.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/gridss/call/main.nf:46:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
