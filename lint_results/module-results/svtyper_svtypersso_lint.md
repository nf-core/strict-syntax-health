# Nextflow lint results

- Generated: 2026-02-14T00:22:37.784990+00:00
- Nextflow version: 26.01.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/svtyper/svtypersso/main.nf:46:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
