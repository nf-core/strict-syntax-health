# Nextflow lint results

- Generated: 2026-02-01T00:22:15.933474+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 error

## :x: Errors

- Error: `modules/nf-core/ichorcna/createpon/main.nf:31:9`: `exons` is already declared

  ```nextflow
      def exons  = exons           ? "exons.bed='${exons}',"                : ''
          ^^^^^^^^^^
  ```
