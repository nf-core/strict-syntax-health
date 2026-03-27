# Nextflow lint results

- Generated: 2026-03-27T00:27:41.786523+00:00
- Nextflow version: 26.03.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/quant_tximport_summarizedexperiment/main.nf:33:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, results -> [ [:], results ] }
                 ^^^^^^^^^^
  ```
