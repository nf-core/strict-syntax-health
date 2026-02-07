# Nextflow lint results

- Generated: 2026-02-07T00:24:15.272396+00:00
- Nextflow version: 25.12.0-edge
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
