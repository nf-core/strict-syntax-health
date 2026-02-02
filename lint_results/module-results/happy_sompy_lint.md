# Nextflow lint results

- Generated: 2026-02-02T00:19:53.398251+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 error

## :x: Errors

- Error: `modules/nf-core/happy/sompy/main.nf:35:9`: `bams` is already declared

  ```nextflow
      def bams = bams ? "--bam ${bams}" : ""
          ^^^^^^^^^^
  ```
