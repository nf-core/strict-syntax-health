# Nextflow lint results

- Generated: 2026-05-27T00:44:41.099370+00:00
- Nextflow version: 26.04.2
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/vcf_impute_minimac4/main.nf:90:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf_index = ch_vcf_index // channel: [ [id, panel, chr], vcf, index ]
      ^^^^^^^^^^
  ```
