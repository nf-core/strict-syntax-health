# Nextflow lint results

- Generated: 2026-02-12T00:24:23.138321+00:00
- Nextflow version: 26.01.1-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/happy/prepy/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/happy/prepy/main.nf:46:9`: Variable was declared but not used

  ```nextflow
      def restrict_region = bed ? "-R ${bed}": ""
          ^^^^^^^^^^
  ```
