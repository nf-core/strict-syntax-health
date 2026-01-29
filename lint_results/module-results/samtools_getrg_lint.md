# Nextflow lint results

- Generated: 2026-01-29T00:22:49.004166+00:00
- Nextflow version: 25.12.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/samtools/getrg/main.nf:28:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/samtools/getrg/main.nf:41:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^^^^^
  ```
