# Nextflow lint results

- Generated: 2026-02-14T00:22:37.753275+00:00
- Nextflow version: 26.01.1-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/porechop/abi/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/porechop/abi/main.nf:46:9`: Variable was declared but not used

  ```nextflow
      def adapters_list = custom_adapters ? "--custom_adapters ${custom_adapters}" : ""
          ^^^^^^^^^^
  ```
