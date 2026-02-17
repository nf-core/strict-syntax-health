# Nextflow lint results

- Generated: 2026-02-17T00:24:27.758788+00:00
- Nextflow version: 26.01.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/motus/preplong/main.nf:49:9`: Variable was declared but not used

  ```nextflow
      def refdb = db ? "-db ${db}" : ""
          ^^^^^^^^^^
  ```
