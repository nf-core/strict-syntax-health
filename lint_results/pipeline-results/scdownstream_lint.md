# Nextflow lint results

- Generated: 2026-04-17T00:31:40.467959992Z
- Nextflow version: 26.03.2-edge
- Summary: 29 warnings

## :warning: Warnings

- Warning: `modules/local/adata/entropy/main.nf:25:5`: Variable was declared but not used

  ```nextflow
      args = task.ext.args ?: ''
      ^^^^
  ```

- Warning: `modules/local/adata/merge/main.nf:26:5`: Variable was declared but not used

  ```nextflow
      force_obs_cols = task.ext.force_obs_cols ?: params.force_obs_cols ?: ""
      ^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/adata/mygene/main.nf:22:5`: Variable was declared but not used

  ```nextflow
      input_col = task.ext.input_col ?: "index"
      ^^^^^^^^^
  ```

- Warning: `modules/local/adata/mygene/main.nf:23:5`: Variable was declared but not used

  ```nextflow
      output_col = task.ext.output_col ?: "symbols"
      ^^^^^^^^^^
  ```

- Warning: `modules/local/liana/rankaggregate/main.nf:22:5`: Variable was declared but not used

  ```nextflow
      args    = task.ext.args   ?: ''
      ^^^^
  ```

- Warning: `modules/local/liana/rankaggregate/main.nf:23:5`: Variable was declared but not used

  ```nextflow
      obs_key = meta.obs_key ?: "leiden"
      ^^^^^^^
  ```

- Warning: `modules/local/scanpy/bbknn/main.nf:23:5`: Variable was declared but not used

  ```nextflow
      args   = task.ext.args ?: ''
      ^^^^
  ```

- Warning: `modules/local/scanpy/combat/main.nf:25:5`: Variable was declared but not used

  ```nextflow
      args   = task.ext.args   ?: ''
      ^^^^
  ```

- Warning: `modules/local/scanpy/harmony/main.nf:22:5`: Variable was declared but not used

  ```nextflow
      args   = task.ext.args ?: ''
      ^^^^
  ```

- Warning: `modules/local/scanpy/hvgs/main.nf:25:5`: Variable was declared but not used

  ```nextflow
      batch_key = task.ext.batch_key ?: ""
      ^^^^^^^^^
  ```

- Warning: `modules/local/scanpy/neighbors/main.nf:23:5`: Variable was declared but not used

  ```nextflow
      args   = task.ext.args ?: ''
      ^^^^
  ```

- Warning: `modules/local/scanpy/paga/main.nf:25:5`: Variable was declared but not used

  ```nextflow
      obs_key = meta.obs_key ?: "leiden"
      ^^^^^^^
  ```

- Warning: `modules/local/scanpy/pca/main.nf:24:5`: Variable was declared but not used

  ```nextflow
      args   = task.ext.args ?: ''
      ^^^^
  ```

- Warning: `modules/local/scanpy/rankgenesgroups/main.nf:28:5`: Variable was declared but not used

  ```nextflow
      args   = task.ext.args ?: ''
      ^^^^
  ```

- Warning: `modules/local/scanpy/umap/main.nf:23:5`: Variable was declared but not used

  ```nextflow
      args   = task.ext.args ?: ''
      ^^^^
  ```

- Warning: `modules/local/scarches/expimap/main.nf:26:5`: Variable was declared but not used

  ```nextflow
      args   = task.ext.args ?: ''
      ^^^^
  ```

- Warning: `modules/local/scvitools/scanvi/main.nf:33:5`: Variable was declared but not used

  ```nextflow
      n_hidden = task.ext.n_hidden ?: 128
      ^^^^^^^^
  ```

- Warning: `modules/local/scvitools/scanvi/main.nf:34:5`: Variable was declared but not used

  ```nextflow
      n_layers = task.ext.n_layers ?: 2
      ^^^^^^^^
  ```

- Warning: `modules/local/scvitools/scanvi/main.nf:35:5`: Variable was declared but not used

  ```nextflow
      n_latent = task.ext.n_latent ?: 30
      ^^^^^^^^
  ```

- Warning: `modules/local/scvitools/scanvi/main.nf:36:5`: Variable was declared but not used

  ```nextflow
      dispersion = task.ext.dispersion ?: 'gene'
      ^^^^^^^^^^
  ```

- Warning: `modules/local/scvitools/scanvi/main.nf:37:5`: Variable was declared but not used

  ```nextflow
      gene_likelihood = task.ext.gene_likelihood ?: 'zinb'
      ^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/scvitools/scanvi/main.nf:38:5`: Variable was declared but not used

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

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```
