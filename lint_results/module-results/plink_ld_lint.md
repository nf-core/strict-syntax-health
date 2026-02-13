# Nextflow lint results

- Generated: 2026-02-13T00:24:57.271365+00:00
- Nextflow version: 26.01.1-edge
- Summary: 4 warnings

## :warning: Warnings

- Warning: `modules/nf-core/plink/ld/main.nf:32:9`: Variable was declared but not used

  ```nextflow
      def outmeta = ""
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/plink/ld/main.nf:65:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/plink/ld/main.nf:66:9`: Variable was declared but not used

  ```nextflow
      def args2 = task.ext.args2 ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/plink/ld/main.nf:71:9`: Variable was declared but not used

  ```nextflow
      def outmeta = ""
          ^^^^^^^^^^
  ```
