# Nextflow lint results

- Generated: 2026-09-22T00:24:48.368005624Z
- Nextflow version: 26.08.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/local/align_cellrangermulti/main.nf:62:9`: Variable was declared but not used

  ```nextflow
          ch_gex_barcodes           = params.gex_barcode_sample_assignment ? file(params.gex_barcode_sample_assignment) : []
          ^^^^^^^^^^^^^^^
  ```
