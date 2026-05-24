# Nextflow lint results

- Generated: 2026-05-24T00:38:50.940763+00:00
- Nextflow version: 26.04.2
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/vcf_impute_beagle5/main.nf:119:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf_index = ch_vcf_index // channel: [ [id, chr, tools], vcf, index ]
      ^^^^^^^^^^
  ```
