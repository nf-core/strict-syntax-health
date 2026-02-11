# Nextflow lint results

- Generated: 2026-02-11T00:30:24.210577+00:00
- Nextflow version: 26.01.0-edge
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
