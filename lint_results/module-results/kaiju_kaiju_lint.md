# Nextflow lint results

- Generated: 2026-02-10T00:27:01.482884+00:00
- Nextflow version: 26.01.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/kaiju/kaiju/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/kaiju/kaiju/main.nf:45:9`: Variable was declared but not used

  ```nextflow
      def input = meta.single_end ? "-i ${reads}" : "-i ${reads[0]} -j ${reads[1]}"
          ^^^^^^^^^^
  ```
