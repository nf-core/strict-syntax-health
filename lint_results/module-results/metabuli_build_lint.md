# Nextflow lint results

- Generated: 2026-03-15T00:24:30.042641+00:00
- Nextflow version: 26.02.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/metabuli/build/main.nf:46:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
