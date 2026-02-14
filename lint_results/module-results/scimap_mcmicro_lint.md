# Nextflow lint results

- Generated: 2026-02-14T00:22:37.769652+00:00
- Nextflow version: 26.01.1-edge
- Summary: 4 warnings

## :warning: Warnings

- Warning: `modules/nf-core/scimap/mcmicro/main.nf:24:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/scimap/mcmicro/main.nf:25:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/scimap/mcmicro/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/scimap/mcmicro/main.nf:45:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^^^^^
  ```
