# Nextflow lint results

- Generated: 2026-07-04T00:37:47.496759+00:00
- Nextflow version: 26.06.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/vcf_impute_beagle5/main.nf:132:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf_index = ch_vcf_index // channel: [ [id, chr, tools], vcf, index ]
      ^^^^^^^^^^
  ```
