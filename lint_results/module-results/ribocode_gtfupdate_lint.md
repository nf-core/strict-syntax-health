# Nextflow lint results

- Generated: 2026-02-03T00:25:25.916100+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/ribocode/gtfupdate/main.nf:32:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
