# Nextflow lint results

- Generated: 2026-02-07T00:24:15.173291+00:00
- Nextflow version: 25.12.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/custom/addmostseverepli/main.nf:45:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/custom/addmostseverepli/main.nf:46:9`: Variable was declared but not used

  ```nextflow
      def args2 = task.ext.args2 ?: ''
          ^^^^^^^^^^
  ```
