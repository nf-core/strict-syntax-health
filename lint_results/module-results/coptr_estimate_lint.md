# Nextflow lint results

- Generated: 2026-02-10T00:27:01.452363+00:00
- Nextflow version: 26.01.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/coptr/estimate/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/coptr/estimate/main.nf:37:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
