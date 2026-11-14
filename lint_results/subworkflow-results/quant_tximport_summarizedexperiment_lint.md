# Nextflow lint results

- Generated: 2026-11-14T00:15:58.885336+00:00
- Nextflow version: 26.10.6
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/quant_tximport_summarizedexperiment/main.nf:68:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { sorted -> [ ['id': 'all_samples'], sorted.collect { it[1] } ] }
                                                                         ^^^^^^^^^^
  ```
