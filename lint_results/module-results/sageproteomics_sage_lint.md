# Nextflow lint results

- Generated: 2026-02-17T00:24:27.786451+00:00
- Nextflow version: 26.01.1-edge
- Summary: 4 warnings

## :warning: Warnings

- Warning: `modules/nf-core/sageproteomics/sage/main.nf:29:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/sageproteomics/sage/main.nf:30:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/sageproteomics/sage/main.nf:48:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/sageproteomics/sage/main.nf:49:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^^^^^
  ```
