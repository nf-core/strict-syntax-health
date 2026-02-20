# Nextflow lint results

- Generated: 2026-02-20T00:23:00.646370+00:00
- Nextflow version: 26.01.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/fastq_taxonomic_profile_metaphlan/main.nf:21:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, profile -> [[id: 'all_samples'], profile] }
                 ^^^^^^^^^^
  ```
