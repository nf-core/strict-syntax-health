# Nextflow lint results

- Generated: 2026-02-02T00:19:53.405123+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/icountmini/segment/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
