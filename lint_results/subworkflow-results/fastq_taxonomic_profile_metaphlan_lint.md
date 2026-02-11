# Nextflow lint results

- Generated: 2026-02-11T00:30:37.454429+00:00
- Nextflow version: 26.01.0-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `subworkflows/nf-core/fastq_taxonomic_profile_metaphlan/main.nf:12:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_taxonomic_profile_metaphlan/main.nf:20:128`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      metaphlan_merged_profiles_txt = METAPHLAN_MERGEMETAPHLANTABLES(METAPHLAN_METAPHLAN.out.profile.map { [[id: 'all_samples'], it[1]] }.groupTuple(sort: { it.getName() })).txt
                                                                                                                                 ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_taxonomic_profile_metaphlan/main.nf:20:156`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      metaphlan_merged_profiles_txt = METAPHLAN_MERGEMETAPHLANTABLES(METAPHLAN_METAPHLAN.out.profile.map { [[id: 'all_samples'], it[1]] }.groupTuple(sort: { it.getName() })).txt
                                                                                                                                                             ^^^^^^^^^^
  ```
