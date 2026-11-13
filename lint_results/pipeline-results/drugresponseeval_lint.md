# Nextflow lint results

- Generated: 2026-11-13T00:14:42.154856823Z
- Nextflow version: 26.10.5
- Summary: 22 warnings

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

- Warning: `conf/modules.config:98:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:106:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:114:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:130:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:154:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:162:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:178:23`: Parameter was not used -- prefix with `_` to suppress warning

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

- Warning: `subworkflows/local/model_testing/main.nf:77:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              .filter { model_name, test_mode, split_id, split_dataset, best_hpams, randomization_views, path_data ->
                                                    ^^^^^^^^^
  ```

- Warning: `subworkflows/local/model_testing/main.nf:77:72`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              .filter { model_name, test_mode, split_id, split_dataset, best_hpams, randomization_views, path_data ->
                                                                         ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/model_testing/main.nf:77:120`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              .filter { model_name, test_mode, split_id, split_dataset, best_hpams, randomization_views, path_data ->
                                                                                                                         ^^^^^^^^^
  ```

- Warning: `subworkflows/local/model_testing/main.nf:171:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              .map{ model_name, final_constant, test_mode, best_hpam_combi ->
                                                ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/run_cv/main.nf:75:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  .filter { cs_name, dataset_path ->
                                            ^^^^^^^
  ```

- Warning: `subworkflows/local/run_cv/main.nf:78:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  .map { cs_name, dataset_path ->
                                         ^^^^^^^
  ```

- Warning: `subworkflows/local/run_cv/main.nf:83:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  .filter { cs_name, dataset_path ->
                                            ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_drugresponseeval_pipeline/main.nf:141:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_models = channel.from(models.split(',').collect { it.trim() })
                                                           ^^
  ```

- Warning: `workflows/drugresponseeval.nf:129:9`: Variable was declared but not used

  ```nextflow
      def ch_collated_versions = softwareVersionsToYAML(ch_versions.mix(topic_versions.versions_file))
          ^^^^^^^^^^^^^^^^^^^^
  ```
