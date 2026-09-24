# Nextflow lint results

- Generated: 2026-09-24T00:23:02.789531+00:00
- Nextflow version: 26.09.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/nf-core/orftable_fasta_gtf_buildorfcatalogue/main.nf:49:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it.size() > 0 }
                    ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/orftable_fasta_gtf_buildorfcatalogue/main.nf:55:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it.size() > 0 }
                    ^^^^^^^^^^
  ```
