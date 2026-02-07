# Nextflow lint results

- Generated: 2026-02-07T00:24:15.181599+00:00
- Nextflow version: 25.12.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/ganon/classify/main.nf:48:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/ganon/classify/main.nf:50:9`: Variable was declared but not used

  ```nextflow
      def input = meta.single_end ? "--single-reads ${fastqs}" : "--paired-reads ${fastqs}"
          ^^^^^^^^^^
  ```
