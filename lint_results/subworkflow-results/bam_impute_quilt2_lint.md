# Nextflow lint results

- Generated: 2026-05-26T00:41:33.182934+00:00
- Nextflow version: 26.04.2
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_impute_quilt2/main.nf:75:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf_index = ch_vcf_index // channel: [ meta, vcf, tbi/csi ]
      ^^^^^^^^^^
  ```
