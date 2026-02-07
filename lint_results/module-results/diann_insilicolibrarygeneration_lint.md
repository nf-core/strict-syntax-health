# Nextflow lint results

- Generated: 2026-02-07T00:24:15.175866+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/diann/insilicolibrarygeneration/main.nf:50:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
