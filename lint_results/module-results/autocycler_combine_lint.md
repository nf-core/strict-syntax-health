# Nextflow lint results

- Generated: 2026-02-01T00:22:15.862291+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/autocycler/combine/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args   ?: ''
          ^^^^^^^^^^
  ```
