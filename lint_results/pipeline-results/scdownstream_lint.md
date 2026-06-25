# Nextflow lint results

- Generated: 2026-06-25T00:43:51.174082932Z
- Nextflow version: 26.05.0-edge
- Summary: 32 warnings

## :warning: Warnings

- Warning: `main.nf:149:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = SCDOWNSTREAM.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/adata/merge/main.nf:26:5`: Variable was declared but not used

  ```nextflow
      force_obs_cols = task.ext.force_obs_cols ?: params.force_obs_cols ?: ""
      ^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/adata/mygene/main.nf:23:5`: Variable was declared but not used

  ```nextflow
      input_col = task.ext.input_col ?: "index"
      ^^^^^^^^^
  ```

- Warning: `modules/local/adata/mygene/main.nf:24:5`: Variable was declared but not used

  ```nextflow
      output_col = task.ext.output_col ?: "symbols"
      ^^^^^^^^^^
  ```

- Warning: `modules/local/liana/rankaggregate/main.nf:22:5`: Variable was declared but not used

  ```nextflow
      obs_key = meta.obs_key ?: "leiden"
      ^^^^^^^
  ```

- Warning: `modules/local/scanpy/hvgs/main.nf:25:5`: Variable was declared but not used

  ```nextflow
      batch_key = task.ext.batch_key ?: ""
      ^^^^^^^^^
  ```

- Warning: `modules/local/scanpy/paga/main.nf:25:5`: Variable was declared but not used

  ```nextflow
      obs_key = meta.obs_key ?: "leiden"
      ^^^^^^^
  ```

- Warning: `modules/local/scarches/expimap/main.nf:26:5`: Variable was declared but not used

  ```nextflow
      args   = task.ext.args ?: ''
      ^^^^
  ```

- Warning: `modules/local/scvitools/scanvi/main.nf:34:5`: Variable was declared but not used

  ```nextflow
      n_hidden = task.ext.n_hidden ?: 128
      ^^^^^^^^
  ```

- Warning: `modules/local/scvitools/scanvi/main.nf:35:5`: Variable was declared but not used

  ```nextflow
      n_layers = task.ext.n_layers ?: 2
      ^^^^^^^^
  ```

- Warning: `modules/local/scvitools/scanvi/main.nf:36:5`: Variable was declared but not used

  ```nextflow
      n_latent = task.ext.n_latent ?: 30
      ^^^^^^^^
  ```

- Warning: `modules/local/scvitools/scanvi/main.nf:37:5`: Variable was declared but not used

  ```nextflow
      dispersion = task.ext.dispersion ?: 'gene'
      ^^^^^^^^^^
  ```

- Warning: `modules/local/scvitools/scanvi/main.nf:38:5`: Variable was declared but not used

  ```nextflow
      gene_likelihood = task.ext.gene_likelihood ?: 'zinb'
      ^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/scvitools/scanvi/main.nf:39:5`: Variable was declared but not used

  ```nextflow
      max_epochs = task.ext.max_epochs ?: null
      ^^^^^^^^^^
  ```

- Warning: `modules/local/scvitools/scvi/main.nf:31:5`: Variable was declared but not used

  ```nextflow
      n_hidden = task.ext.n_hidden ?: 128
      ^^^^^^^^
  ```

- Warning: `modules/local/scvitools/scvi/main.nf:32:5`: Variable was declared but not used

  ```nextflow
      n_layers = task.ext.n_layers ?: 2
      ^^^^^^^^
  ```

- Warning: `modules/local/scvitools/scvi/main.nf:33:5`: Variable was declared but not used

  ```nextflow
      n_latent = task.ext.n_latent ?: 30
      ^^^^^^^^
  ```

- Warning: `modules/local/scvitools/scvi/main.nf:34:5`: Variable was declared but not used

  ```nextflow
      dispersion = task.ext.dispersion ?: 'gene'
      ^^^^^^^^^^
  ```

- Warning: `modules/local/scvitools/scvi/main.nf:35:5`: Variable was declared but not used

  ```nextflow
      gene_likelihood = task.ext.gene_likelihood ?: 'zinb'
      ^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/scvitools/scvi/main.nf:36:5`: Variable was declared but not used

  ```nextflow
      max_epochs = task.ext.max_epochs ?: null
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/ambient_correction/main.nf:111:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      h5ad     = ch_h5ad     // channel: [ meta, h5ad ]
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/celltype_assignment/main.nf:39:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      obs      = ch_obs      // channel: [ meta, pkl ]
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/cluster_targets/main.nf:48:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      targets = ch_targets // channel: [ meta, h5ad ]
      ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/load_h5ad/main.nf:75:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      h5ad     = ch_output   // channel: [ meta, h5ad, h5ad ]
      ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/pseudobulking/main.nf:22:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      h5ad_pseudobulk = ch_h5ad_pseudobulk // channel: [ integration, h5ad ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/singler/main.nf:43:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      obs      = ch_obs
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/unify_genes/main.nf:36:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      h5ad = ch_h5ad // channel: [ meta, h5ad ]
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_scdownstream_pipeline/main.nf:183:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      if (!rows || rows.any { !it.analyses }) {
                               ^^
  ```

- Warning: `subworkflows/nf-core/h5ad_removebackground_barcodes_cellbender_anndata/main.nf:18:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      h5ad = ANNDATA_BARCODES.out.h5ad  // channel: [ val(meta), path(h5ad) ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nextflow_pipeline/main.nf:43:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:20:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      valid_config = valid_config
      ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:72:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```
