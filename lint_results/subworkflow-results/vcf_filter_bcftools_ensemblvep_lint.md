# Nextflow lint results

- Generated: 2026-02-07T00:24:27.406282+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/vcf_filter_bcftools_ensemblvep/main.nf:14:5`: Variable was declared but not used

  ```nextflow
      ch_versions = channel.empty()
      ^^^^^^^^^^
  ```
