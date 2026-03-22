# Nextflow lint results

- Generated: 2026-03-22T00:21:34.732905+00:00
- Nextflow version: 26.03.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/quant_tximport_summarizedexperiment/main.nf:33:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, results -> [ [:], results ] }
                 ^^^^^^^^^^
  ```
