# Nextflow lint results

- Generated: 2026-06-16T19:24:09.731353463Z
- Nextflow version: 26.04.3
- Summary: 32 warnings

## :warning: Warnings

- Warning: `conf/modules.config:65:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:73:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:81:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:89:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:97:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:105:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:114:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:134:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:161:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:209:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:217:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:244:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `main.nf:52:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions = ch_versions
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/model_testing/main.nf:63:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          .map{ model_class, model_name, rand_file -> [model_name, rand_file] }
                                ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/model_testing/main.nf:74:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              .filter { model_name, test_mode, split_id, split_dataset, best_hpams, randomization_views, path_data ->
                                                    ^^^^^^^^^
  ```

- Warning: `subworkflows/local/model_testing/main.nf:74:72`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              .filter { model_name, test_mode, split_id, split_dataset, best_hpams, randomization_views, path_data ->
                                                                         ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/model_testing/main.nf:74:120`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              .filter { model_name, test_mode, split_id, split_dataset, best_hpams, randomization_views, path_data ->
                                                                                                                         ^^^^^^^^^
  ```

- Warning: `subworkflows/local/model_testing/main.nf:142:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              .map { model_class, model_name, train_ds, val_ds, es_ds ->
                                     ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/model_testing/main.nf:162:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              .map{ model_name, final_constant, test_mode, best_hpam_combi ->
                                                ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/model_testing/main.nf:175:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          .map{ test_mode, model, pred_file -> [test_mode, model.split("\\.")[0]] }
                                                  ^^^^^^^^^
  ```

- Warning: `subworkflows/local/model_testing/main.nf:222:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions = ch_versions
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/run_cv/main.nf:54:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  .filter { dataset_name, dataset_path ->
                                            ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/run_cv/main.nf:57:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  .map { dataset_name, dataset_path ->
                                         ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/run_cv/main.nf:62:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  .filter { dataset_name, dataset_path ->
                                            ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/run_cv/main.nf:131:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { model_class, model_name, hpam_combis -> [model_name, hpam_combis] }
                 ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/run_cv/main.nf:139:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { model_class, model_name, test_mode, split -> [model_name, test_mode, split] }
                 ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_drugresponseeval_pipeline/main.nf:138:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_models = channel.from(models.split(',').collect { it.trim() })
                                                           ^^
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

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:76:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/drugresponseeval.nf:90:9`: Variable was declared but not used

  ```nextflow
      def ch_collated_versions = softwareVersionsToYAML(ch_versions.mix(topic_versions.versions_file))
          ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/drugresponseeval.nf:99:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions       = ch_versions                 // channel: [ path(versions.yml) ]
      ^^^^^^^^^^^^^^^^^^^^
  ```
