# Nextflow lint results

- Generated: 2026-03-01T00:23:46.131791+00:00
- Nextflow version: 26.02.0-edge
- Summary: 1 error

## :x: Errors

- Error: `modules/nf-core/samtools/addreplacerg/main.nf:49:9`: `file_type` is already declared

  ```nextflow
      def file_type = input.getExtension()
          ^^^^^^^^^^
  ```
