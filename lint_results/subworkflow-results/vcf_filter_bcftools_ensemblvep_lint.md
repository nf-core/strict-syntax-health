# Nextflow lint results

- Generated: 2026-02-10T00:27:13.423652+00:00
- Nextflow version: 26.01.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/vcf_filter_bcftools_ensemblvep/main.nf:14:5`: Variable was declared but not used

  ```nextflow
      ch_versions = channel.empty()
      ^^^^^^^^^^
  ```
