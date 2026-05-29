# Nextflow lint results

- Generated: 2026-05-29T00:45:51.867676+00:00
- Nextflow version: 26.04.3
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_impute_quilt2/main.nf:75:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf_index = ch_vcf_index // channel: [ meta, vcf, tbi/csi ]
      ^^^^^^^^^^
  ```
