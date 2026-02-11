# Nextflow lint results

- Generated: 2026-02-11T00:30:24.159806+00:00
- Nextflow version: 26.01.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/iphop/predict/main.nf:25:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/iphop/predict/main.nf:48:9`: Variable was declared but not used

  ```nextflow
      def prefix    = task.ext.prefix ?: "${meta.id}"
          ^^^^^^^^^^
  ```
