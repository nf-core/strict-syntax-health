# Nextflow lint results

- Generated: 2026-07-16T00:33:22.644610+00:00
- Nextflow version: 26.06.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_tumor_normal_somatic_variant_calling_strelka/main.nf:52:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf      = ch_vcf
      ^^^^^^^^^^
  ```
