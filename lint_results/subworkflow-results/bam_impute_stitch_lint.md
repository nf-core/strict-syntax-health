# Nextflow lint results

- Generated: 2026-05-27T00:44:41.087728+00:00
- Nextflow version: 26.04.2
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_impute_stitch/main.nf:88:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf_index = ch_vcf_index // channel:   [ [id, chr], vcf, tbi ]
      ^^^^^^^^^^
  ```
