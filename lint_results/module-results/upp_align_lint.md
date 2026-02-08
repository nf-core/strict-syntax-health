# Nextflow lint results

- Generated: 2026-02-08T00:29:10.374744+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/upp/align/main.nf:24:9`: Variable was declared but not used

  ```nextflow
      def tree_args = tree ? "-t $tree" : ""
          ^^^^^^^^^^
  ```
