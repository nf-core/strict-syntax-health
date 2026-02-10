# Nextflow lint results

- Generated: 2026-02-10T00:27:01.484884+00:00
- Nextflow version: 26.01.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/kmcp/search/main.nf:24:9`: Variable was declared but not used

  ```nextflow
      def input  = meta.single_end ? "${reads}": "-1 ${reads[0]} -2 ${reads[1]}"
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/kmcp/search/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
