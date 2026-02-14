# Nextflow lint results

- Generated: 2026-02-14T00:22:37.722657+00:00
- Nextflow version: 26.01.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/motus/preplong/main.nf:49:9`: Variable was declared but not used

  ```nextflow
      def refdb = db ? "-db ${db}" : ""
          ^^^^^^^^^^
  ```
