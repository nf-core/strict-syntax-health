# Nextflow lint results

- Generated: 2026-02-02T00:19:53.347094+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/cnvpytor/callcnvs/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def bins = bin_sizes ? "-call $bin_sizes" : '-call 1000'
          ^^^^^^^^^^
  ```
