# Nextflow lint results

- Generated: 2026-02-10T00:27:01.503426+00:00
- Nextflow version: 26.01.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/paftools/sam2paf/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args    = task.ext.args     ?: ""
          ^^^^^^^^^^
  ```
