# Nextflow lint results

- Generated: 2026-06-28T00:43:03.827869+00:00
- Nextflow version: 26.05.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_impute_stitch/main.nf:101:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf_index = ch_vcf_index // channel:   [ [id, chr], vcf, tbi ]
      ^^^^^^^^^^
  ```
