# Nextflow lint results

- Generated: 2026-06-16T14:40:40.100657+00:00
- Nextflow version: 26.04.3
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/h5ad_removebackground_barcodes_cellbender_anndata/main.nf:18:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      h5ad = ANNDATA_BARCODES.out.h5ad  // channel: [ val(meta), path(h5ad) ]
      ^^^^^^^^^^
  ```
