# Nextflow lint results

- Generated: 2026-02-10T00:27:01.539471+00:00
- Nextflow version: 26.01.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/tcoffee/alncompare/main.nf:54:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
