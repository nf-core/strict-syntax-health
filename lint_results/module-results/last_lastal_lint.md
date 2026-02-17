# Nextflow lint results

- Generated: 2026-02-17T00:24:27.744003+00:00
- Nextflow version: 26.01.1-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/last/lastal/main.nf:94:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/last/lastal/main.nf:96:9`: Variable was declared but not used

  ```nextflow
      def trained_params = param_file ? "-p ${param_file}"  : ''
          ^^^^^^^^^^
  ```
