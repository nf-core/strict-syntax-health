# Nextflow lint results

- Generated: 2026-07-01T00:52:40.514632+00:00
- Nextflow version: 26.05.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_impute_quilt2/main.nf:86:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf_index = ch_vcf_index // channel: [ meta, vcf, tbi/csi ]
      ^^^^^^^^^^
  ```
