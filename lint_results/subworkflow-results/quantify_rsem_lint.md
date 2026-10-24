# Nextflow lint results

- Generated: 2026-10-24T00:27:19.447255+00:00
- Nextflow version: 26.10.3
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/nf-core/quantify_rsem/main.nf:62:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .map { sorted -> [ ['id': 'all_samples'], sorted.collect { it[1] } ] },
                                                                             ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/quantify_rsem/main.nf:66:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .map { sorted -> sorted.collect { it[1] } }
                                                    ^^^^^^^^^
  ```
