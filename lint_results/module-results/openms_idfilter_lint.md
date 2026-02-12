# Nextflow lint results

- Generated: 2026-02-12T00:24:23.156946+00:00
- Nextflow version: 26.01.1-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/openms/idfilter/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/openms/idfilter/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def filter = filter_file ? "${filter_citerion} ${filter_file}" : ""
          ^^^^^^^^^^
  ```
