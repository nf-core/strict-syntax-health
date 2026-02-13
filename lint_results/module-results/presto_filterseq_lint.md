# Nextflow lint results

- Generated: 2026-02-13T00:24:57.274684+00:00
- Nextflow version: 26.01.1-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `modules/nf-core/presto/filterseq/main.nf:25:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/presto/filterseq/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/presto/filterseq/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^^^^^
  ```
