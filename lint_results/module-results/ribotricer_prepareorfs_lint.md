# Nextflow lint results

- Generated: 2026-02-13T00:24:57.282341+00:00
- Nextflow version: 26.01.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/ribotricer/prepareorfs/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
