# Nextflow lint results

- Generated: 2026-02-08T00:29:10.365320+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/ska/distance/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args         = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
