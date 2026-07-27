# Nextflow lint results

- Generated: 2026-07-27T00:34:23.551410961Z
- Nextflow version: 26.07.0-edge
- Summary: 21 warnings

## :warning: Warnings

- Warning: `modules/local/adata/merge/main.nf:24:5`: Variable was declared but not used

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

- Warning: `modules/local/liana/rankaggregate/main.nf:26:5`: Variable was declared but not used

  ```nextflow
      obs_key = meta.obs_key ?: "leiden"
      ^^^^^^^
  ```

- Warning: `modules/local/scanpy/hvgs/main.nf:27:5`: Variable was declared but not used

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

- Warning: `modules/local/scvitools/scanvi/main.nf:40:5`: Variable was declared but not used

  ```nextflow
      use_observed_lib_size = task.ext.use_observed_lib_size != null ? task.ext.use_observed_lib_size : true
      ^^^^^^^^^^^^^^^^^^^^^
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

- Warning: `modules/local/scvitools/scvi/main.nf:37:5`: Variable was declared but not used

  ```nextflow
      use_observed_lib_size = task.ext.use_observed_lib_size != null ? task.ext.use_observed_lib_size : true
      ^^^^^^^^^^^^^^^^^^^^^
  ```
