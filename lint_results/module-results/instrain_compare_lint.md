# Nextflow lint results

- Generated: 2026-02-11T00:30:24.159078+00:00
- Nextflow version: 26.01.0-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `modules/nf-core/instrain/compare/main.nf:28:9`: Variable was declared but not used

  ```nextflow
      def stb_args = stb_file ? "-s ${stb_file}": ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/instrain/compare/main.nf:45:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/instrain/compare/main.nf:47:9`: Variable was declared but not used

  ```nextflow
      def stb_args = stb_file ? "-s ${stb_file}": ''
          ^^^^^^^^^^
  ```
