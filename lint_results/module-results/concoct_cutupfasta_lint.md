# Nextflow lint results

- Generated: 2026-02-02T00:19:53.348669+00:00
- Nextflow version: 25.12.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/concoct/cutupfasta/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/concoct/cutupfasta/main.nf:45:9`: Variable was declared but not used

  ```nextflow
      def bedfile = bed ? "-b ${prefix}.bed" : ""
          ^^^^^^^^^^
  ```
