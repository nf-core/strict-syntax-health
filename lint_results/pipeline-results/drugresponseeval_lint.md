# Nextflow lint results

- Generated: 2026-10-28T00:15:30.301525968Z
- Nextflow version: 26.10.4
- Summary: 27 warnings

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

- Warning: `modules/nf-core/custom/dumpsoftwareversions/main.nf:16:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/unzip/main.nf:16:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `subworkflows/local/model_testing/main.nf:61:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          .map{ model_class, model_name, rand_file -> [model_name, rand_file] }
                                ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/model_testing/main.nf:72:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              .filter { model_name, test_mode, split_id, split_dataset, best_hpams, randomization_views, path_data ->
                                                    ^^^^^^^^^
  ```

- Warning: `subworkflows/local/model_testing/main.nf:72:72`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              .filter { model_name, test_mode, split_id, split_dataset, best_hpams, randomization_views, path_data ->
                                                                         ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/model_testing/main.nf:72:120`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              .filter { model_name, test_mode, split_id, split_dataset, best_hpams, randomization_views, path_data ->
                                                                                                                         ^^^^^^^^^
  ```

- Warning: `subworkflows/local/model_testing/main.nf:154:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              .map{ model_name, final_constant, test_mode, best_hpam_combi ->
                                                ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/model_testing/main.nf:166:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          .map{ test_mode, model, pred_file -> [test_mode, model.split("\\.")[0]] }
                                                  ^^^^^^^^^
  ```

- Warning: `subworkflows/local/run_cv/main.nf:59:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  .filter { dataset_name, dataset_path ->
                                            ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/run_cv/main.nf:62:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  .map { dataset_name, dataset_path ->
                                         ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/run_cv/main.nf:67:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  .filter { dataset_name, dataset_path ->
                                            ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/run_cv/main.nf:133:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { model_class, model_name, hpam_combis -> [model_name, hpam_combis] }
                 ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/run_cv/main.nf:141:16`: Parameter was not used -- prefix with `_` to suppress warning

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
