# Nextflow lint results

- Generated: 2026-06-16T19:48:59.560949+00:00
- Nextflow version: 26.04.3
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_impute_stitch/main.nf:101:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf_index = ch_vcf_index // channel:   [ [id, chr], vcf, tbi ]
      ^^^^^^^^^^
  ```
