# Nextflow lint results

- Generated: 2026-02-13T00:24:57.250850+00:00
- Nextflow version: 26.01.1-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/mirtop/stats/main.nf:24:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/mirtop/stats/main.nf:39:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
