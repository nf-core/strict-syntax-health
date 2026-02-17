# Nextflow lint results

- Generated: 2026-02-17T00:24:27.752024+00:00
- Nextflow version: 26.01.1-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/metacache/query/main.nf:47:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/metacache/query/main.nf:49:9`: Variable was declared but not used

  ```nextflow
      def input_file = meta.single_end ? reads : "${reads[0]} ${reads[1]} -pairfiles"
          ^^^^^^^^^^
  ```
