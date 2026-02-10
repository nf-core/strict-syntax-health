# Nextflow lint results

- Generated: 2026-02-10T00:27:01.503321+00:00
- Nextflow version: 26.01.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/osfclient/fetch/main.nf:36:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
