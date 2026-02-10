# Nextflow lint results

- Generated: 2026-02-10T00:27:01.453944+00:00
- Nextflow version: 26.01.0-edge
- Summary: 4 warnings

## :warning: Warnings

- Warning: `modules/nf-core/ctatsplicing/prepgenomelib/main.nf:24:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/ctatsplicing/prepgenomelib/main.nf:25:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/ctatsplicing/prepgenomelib/main.nf:39:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/ctatsplicing/prepgenomelib/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^^^^^
  ```
