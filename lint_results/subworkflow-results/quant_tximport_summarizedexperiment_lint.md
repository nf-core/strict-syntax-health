# Nextflow lint results

- Generated: 2026-10-01T00:28:29.776211+00:00
- Nextflow version: 26.09.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/quant_tximport_summarizedexperiment/main.nf:65:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { sorted -> [ ['id': 'all_samples'], sorted.collect { it[1] } ] }
                                                                         ^^^^^^^^^^
  ```
