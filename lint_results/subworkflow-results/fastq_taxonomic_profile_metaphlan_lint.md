# Nextflow lint results

- Generated: 2026-06-13T00:52:48.877837+00:00
- Nextflow version: 26.04.3
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/fastq_taxonomic_profile_metaphlan/main.nf:22:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      merged_taxa = metaphlan_merged_profiles_txt
      ^^^^^^^^^^
  ```
