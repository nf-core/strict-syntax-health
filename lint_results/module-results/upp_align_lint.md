# Nextflow lint results

- Generated: 2026-01-22T00:21:30.805183+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/upp/align/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def tree_args = tree ? "-t $tree" : ""
          ^^^^^^^^^^
  ```
