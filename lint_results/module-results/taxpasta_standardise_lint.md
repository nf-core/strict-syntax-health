# Nextflow lint results

- Generated: 2026-02-14T00:22:37.786934+00:00
- Nextflow version: 26.01.1-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/taxpasta/standardise/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/taxpasta/standardise/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def taxonomy_option = taxonomy ? "--taxonomy ${taxonomy}" : ''
          ^^^^^^^^^^
  ```
