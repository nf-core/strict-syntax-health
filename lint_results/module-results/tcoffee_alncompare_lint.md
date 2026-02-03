# Nextflow lint results

- Generated: 2026-02-03T00:25:25.948169+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/tcoffee/alncompare/main.nf:58:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
