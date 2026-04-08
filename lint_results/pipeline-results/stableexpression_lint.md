# Nextflow lint results

- Generated: 2026-04-08T00:28:01.518332396Z
- Nextflow version: 26.03.2-edge
- Summary: 35 warnings

## :warning: Warnings

- Warning: `modules/local/compute_dataset_statistics/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.dataset}"
          ^^^^^^
  ```

- Warning: `modules/local/expressionatlas/getaccessions/main.nf:31:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def keywords_string = keywords.split(',').collect { it.trim() }.join(' ')
                                                          ^^
  ```

- Warning: `modules/local/geo/getaccessions/main.nf:33:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def keywords_string = keywords.split(',').collect { it.trim() }.join(' ')
                                                          ^^
  ```

- Warning: `subworkflows/local/download_public_datasets/main.nf:24:5`: Variable was declared but not used

  ```nextflow
      ch_fetched_accessions = channel.empty()
      ^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/expression_normalisation/main.nf:31:15`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          meta, file ->
                ^^^^
  ```

- Warning: `subworkflows/local/expression_normalisation/main.nf:36:74`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_raw_rnaseq_datasets_to_normalise = ch_datasets.raw.filter { meta, file -> meta.platform == 'rnaseq' }
                                                                           ^^^^
  ```

- Warning: `subworkflows/local/genorm/main.nf:96:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, i, file_i, j, file_j -> i <= j } // keeps only pairs where i <= j
                  ^^^^
  ```

- Warning: `subworkflows/local/genorm/main.nf:96:26`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, i, file_i, j, file_j -> i <= j } // keeps only pairs where i <= j
                           ^^^^^^
  ```

- Warning: `subworkflows/local/genorm/main.nf:96:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, i, file_i, j, file_j -> i <= j } // keeps only pairs where i <= j
                                      ^^^^^^
  ```

- Warning: `subworkflows/local/get_public_accessions/main.nf:77:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          .filter { species_name, quota -> quota == "ok" }
                                    ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/get_public_accessions/main.nf:78:46`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          .map { species_name, quota -> species_name }
                                               ^^^^^
  ```

- Warning: `subworkflows/local/get_public_accessions/main.nf:114:55`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                      .map { accession, excluded_accessions -> accession }
                                                        ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/idmapping/main.nf:63:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                  .map { it.trim() }
                                         ^^
  ```

- Warning: `subworkflows/local/merge_data/main.nf:25:71`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_normalised_rnaseq_counts = ch_normalised_counts.filter { meta, file -> meta.platform == "rnaseq" }
                                                                        ^^^^
  ```

- Warning: `subworkflows/local/merge_data/main.nf:26:75`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_normalised_microarray_counts = ch_normalised_counts.filter { meta, file -> meta.platform == "microarray" }
                                                                            ^^^^
  ```

- Warning: `subworkflows/local/merge_data/main.nf:29:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                      .map { meta, file -> file }
                                             ^^^^
  ```

- Warning: `subworkflows/local/merge_data/main.nf:34:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                          .map { meta, file -> file }
                                                 ^^^^
  ```

- Warning: `subworkflows/local/merge_data/main.nf:49:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                      .map { meta, file -> file }
                                             ^^^^
  ```

- Warning: `subworkflows/local/merge_data/main.nf:71:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              meta, file -> // extracts design file and adds batch column whenever missing (for custom datasets)
                                    ^^^^
  ```

- Warning: `subworkflows/local/reporting/main.nf:46:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          .map { it.trim() }
                                 ^^
  ```

- Warning: `subworkflows/local/reporting/main.nf:47:35`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          .filter { it != "" }
                                    ^^
  ```

- Warning: `subworkflows/local/reporting/main.nf:57:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_all_counts.map{ meta, file -> file }.collect(),
                             ^^^^
  ```

- Warning: `subworkflows/local/reporting/main.nf:76:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_all_counts.map{ meta, file -> file }.collect(),
                             ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_stableexpression_pipeline/main.nf:31:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_stableexpression_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_stableexpression_pipeline/main.nf:235:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, file ->
                    ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_stableexpression_pipeline/main.nf:252:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, file ->
                 ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_stableexpression_pipeline/main.nf:354:13`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              it.get(1).size() == 2 // only groups with two files
              ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_stableexpression_pipeline/main.nf:357:13`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, files ->
              ^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:101:98`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      return ch_versions.unique().map { version -> processVersionsFromYAML(version) }.unique().mix(Channel.of(workflowVersionToYAML()))
                                                                                                   ^^^^^^^
  ```

- Warning: `workflows/stableexpression.nf:44:5`: Variable was declared but not used

  ```nextflow
      ch_most_stable_genes_summary           = channel.empty()
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/stableexpression.nf:45:5`: Variable was declared but not used

  ```nextflow
      ch_all_genes_statistics                = channel.empty()
      ^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/stableexpression.nf:46:5`: Variable was declared but not used

  ```nextflow
      ch_most_stable_genes_transposed_counts = channel.empty()
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/stableexpression.nf:187:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_all_imputed_counts.map{ meta, file -> file },
                                         ^^^^
  ```
