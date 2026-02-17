# Nextflow lint results

- Generated: 2026-02-17T00:24:41.087617+00:00
- Nextflow version: 26.01.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/vcf_filter_bcftools_ensemblvep/main.nf:14:5`: Variable was declared but not used

  ```nextflow
      ch_versions = channel.empty()
      ^^^^^^^^^^
  ```
