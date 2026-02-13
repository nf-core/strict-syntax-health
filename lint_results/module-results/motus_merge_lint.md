# Nextflow lint results

- Generated: 2026-02-13T00:24:57.253526+00:00
- Nextflow version: 26.01.1-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `modules/nf-core/motus/merge/main.nf:47:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/motus/merge/main.nf:49:9`: Variable was declared but not used

  ```nextflow
      def cmd_input = input.size() > 1 ? "-i ${input.join(',')}" : input.isDirectory() ? "-d ${input}" : "-i ${input}"
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/motus/merge/main.nf:50:9`: Variable was declared but not used

  ```nextflow
      def suffix = task.ext.args?.contains("-B") ? "biom" : "txt"
          ^^^^^^^^^^
  ```
