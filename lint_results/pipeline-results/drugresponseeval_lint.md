# Nextflow lint results

- Generated: 2026-10-10T00:21:57.755132289Z
- Nextflow version: 26.09.2-edge
- Summary: 25 warnings

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

- Warning: `conf/modules.config:122:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:138:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:162:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:170:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:186:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
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

- Warning: `subworkflows/local/model_testing/main.nf:161:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              .map{ model_name, final_constant, test_mode, best_hpam_combi ->
                                                ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/model_testing/main.nf:174:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          .map{ test_mode, model, pred_file -> [test_mode, model.split("\\.")[0]] }
                                                  ^^^^^^^^^
  ```

- Warning: `subworkflows/local/run_cv/main.nf:52:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  .filter { dataset_name, dataset_path ->
                                            ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/run_cv/main.nf:55:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  .map { dataset_name, dataset_path ->
                                         ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/run_cv/main.nf:60:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  .filter { dataset_name, dataset_path ->
                                            ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/run_cv/main.nf:132:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { model_class, model_name, hpam_combis -> [model_name, hpam_combis] }
                 ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/run_cv/main.nf:140:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { model_class, model_name, test_mode, split -> [model_name, test_mode, split] }
                 ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_drugresponseeval_pipeline/main.nf:139:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_models = channel.from(models.split(',').collect { it.trim() })
                                                           ^^
  ```

- Warning: `workflows/drugresponseeval.nf:90:9`: Variable was declared but not used

  ```nextflow
      def ch_collated_versions = softwareVersionsToYAML(ch_versions.mix(topic_versions.versions_file))
          ^^^^^^^^^^^^^^^^^^^^
  ```
