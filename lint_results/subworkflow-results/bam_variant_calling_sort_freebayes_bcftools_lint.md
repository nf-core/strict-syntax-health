# Nextflow lint results

- Generated: 2026-06-20T00:42:56.004730+00:00
- Nextflow version: 26.05.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_variant_calling_sort_freebayes_bcftools/main.nf:27:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf_index      = BCFTOOLS_SORT.out.vcf.join(BCFTOOLS_SORT.out.index) // channel: [ val(meta), path(vcf), path(index) ]
      ^^^^^^^^^^
  ```
