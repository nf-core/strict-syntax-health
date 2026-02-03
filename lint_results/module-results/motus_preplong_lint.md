# Nextflow lint results

- Generated: 2026-02-03T00:25:25.885020+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/motus/preplong/main.nf:49:9`: Variable was declared but not used

  ```nextflow
      def refdb = db ? "-db ${db}" : ""
          ^^^^^^^^^^
  ```
