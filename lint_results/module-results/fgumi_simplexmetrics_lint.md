# Nextflow lint results

- Generated: 2026-07-15T00:27:35.304232+00:00
- Nextflow version: 26.06.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/fgumi/simplexmetrics/main.nf:37:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
