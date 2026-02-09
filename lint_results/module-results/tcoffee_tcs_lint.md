# Nextflow lint results

- Generated: 2026-02-09T00:23:26.258007+00:00
- Nextflow version: 26.01.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/tcoffee/tcs/main.nf:24:9`: Variable was declared but not used

  ```nextflow
      def args          = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/tcoffee/tcs/main.nf:58:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
