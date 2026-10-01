# Nextflow lint results

- Generated: 2026-10-01T00:28:12.102911+00:00
- Nextflow version: 26.09.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/parabricks/deepsomatic/main.nf:47:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
