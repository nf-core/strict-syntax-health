# Nextflow lint results

- Generated: 2026-02-14T00:22:37.668395+00:00
- Nextflow version: 26.01.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/cnvpytor/callcnvs/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def bins = bin_sizes ? "-call $bin_sizes" : '-call 1000'
          ^^^^^^^^^^
  ```
