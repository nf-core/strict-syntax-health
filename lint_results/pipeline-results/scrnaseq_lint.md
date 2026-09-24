# Nextflow lint results

- Generated: 2026-09-24T00:21:49.549159431Z
- Nextflow version: 26.09.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/local/align_cellrangermulti/main.nf:62:9`: Variable was declared but not used

  ```nextflow
          ch_gex_barcodes           = params.gex_barcode_sample_assignment ? file(params.gex_barcode_sample_assignment) : []
          ^^^^^^^^^^^^^^^
  ```
