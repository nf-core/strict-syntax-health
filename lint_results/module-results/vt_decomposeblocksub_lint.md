# Nextflow lint results

- Generated: 2026-02-08T00:29:10.377997+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/vt/decomposeblocksub/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def args2 = task.ext.args2 ?: ''
          ^^^^^^^^^^
  ```
