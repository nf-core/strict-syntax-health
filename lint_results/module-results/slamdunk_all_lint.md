# Nextflow lint results

- Generated: 2026-02-07T00:24:15.265501+00:00
- Nextflow version: 25.12.0-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `modules/nf-core/slamdunk/all/main.nf:31:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/slamdunk/all/main.nf:51:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/slamdunk/all/main.nf:53:9`: Variable was declared but not used

  ```nextflow
      def filterbed = filter_bed ? "-fb ${filter_bed}" : ""
          ^^^^^^^^^^
  ```
