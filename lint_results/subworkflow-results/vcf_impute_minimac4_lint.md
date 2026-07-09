# Nextflow lint results

- Generated: 2026-07-09T00:37:14.348417+00:00
- Nextflow version: 26.06.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/vcf_impute_minimac4/main.nf:119:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf_index = ch_vcf_index // channel: [ [id, panel, chr], vcf, index ]
      ^^^^^^^^^^
  ```
