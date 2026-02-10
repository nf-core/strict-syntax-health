# Nextflow lint results

- Generated: 2026-02-10T00:27:01.454259+00:00
- Nextflow version: 26.01.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/custom/addmostsevereconsequence/main.nf:48:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/custom/addmostsevereconsequence/main.nf:49:9`: Variable was declared but not used

  ```nextflow
      def args2 = task.ext.args2 ?: ''
          ^^^^^^^^^^
  ```
