# Nextflow lint results

- Generated: 2026-02-11T00:30:24.149022+00:00
- Nextflow version: 26.01.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/gt/suffixerator/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def args        = task.ext.args     ?: ''
          ^^^^^^^^^^
  ```
