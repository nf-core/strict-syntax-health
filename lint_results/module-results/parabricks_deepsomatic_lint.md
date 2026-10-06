# Nextflow lint results

- Generated: 2026-10-06T00:25:42.760950+00:00
- Nextflow version: 26.09.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/parabricks/deepsomatic/main.nf:47:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
