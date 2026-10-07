# Nextflow lint results

- Generated: 2026-10-07T00:23:46.212113578Z
- Nextflow version: 26.09.2-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `subworkflows/nf-core/quant_tximport_summarizedexperiment/main.nf:65:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { sorted -> [ ['id': 'all_samples'], sorted.collect { it[1] } ] }
                                                                         ^^
  ```

- Warning: `subworkflows/nf-core/quantify_rsem/main.nf:62:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .map { sorted -> [ ['id': 'all_samples'], sorted.collect { it[1] } ] },
                                                                             ^^
  ```

- Warning: `subworkflows/nf-core/quantify_rsem/main.nf:66:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .map { sorted -> sorted.collect { it[1] } }
                                                    ^^
  ```
