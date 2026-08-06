# Nextflow lint results

- Generated: 2026-08-06T00:29:59.364147622Z
- Nextflow version: 26.07.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/local/align_cellrangermulti/main.nf:62:9`: Variable was declared but not used

  ```nextflow
          ch_gex_barcodes           = params.gex_barcode_sample_assignment ? file(params.gex_barcode_sample_assignment) : []
          ^^^^^^^^^^^^^^^
  ```
