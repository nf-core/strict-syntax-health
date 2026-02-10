# Nextflow lint results

- Generated: 2026-02-10T00:27:01.449881+00:00
- Nextflow version: 26.01.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/cnvpytor/callcnvs/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def bins = bin_sizes ? "-call $bin_sizes" : '-call 1000'
          ^^^^^^^^^^
  ```
