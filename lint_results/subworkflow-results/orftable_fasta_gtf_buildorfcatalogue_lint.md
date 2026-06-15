# Nextflow lint results

- Generated: 2026-06-15T00:46:19.978395+00:00
- Nextflow version: 26.04.3
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/nf-core/orftable_fasta_gtf_buildorfcatalogue/main.nf:44:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it.size() > 0 }
                    ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/orftable_fasta_gtf_buildorfcatalogue/main.nf:50:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it.size() > 0 }
                    ^^^^^^^^^^
  ```
