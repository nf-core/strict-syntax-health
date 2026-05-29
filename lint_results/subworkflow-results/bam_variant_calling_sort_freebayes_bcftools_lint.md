# Nextflow lint results

- Generated: 2026-05-29T00:45:51.869789+00:00
- Nextflow version: 26.04.3
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_variant_calling_sort_freebayes_bcftools/main.nf:27:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf_index      = BCFTOOLS_SORT.out.vcf.join(BCFTOOLS_SORT.out.index) // channel: [ val(meta), path(vcf), path(index) ]
      ^^^^^^^^^^
  ```
