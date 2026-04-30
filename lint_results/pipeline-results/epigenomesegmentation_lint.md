# Nextflow lint results

- Generated: 2026-04-29T00:36:01.554013461Z
- Nextflow version: 26.03.4-edge
- Summary: 78 warnings

## :warning: Warnings

- Warning: `modules/local/distfit_histone_assess/main.nf:10:30`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/src:${projectDir}/bin/HMM/build;
                               ^^^^^^^^^^
  ```

- Warning: `modules/local/distfit_histone_assess/main.nf:10:52`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/src:${projectDir}/bin/HMM/build;
                                                     ^^^^^^^^^^
  ```

- Warning: `modules/local/distfit_histone_assess/main.nf:11:51`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PYTHONPATH=\$PYTHONPATH:/app/src:${projectDir}/bin/src
                                                    ^^^^^^^^^^
  ```

- Warning: `modules/local/distfit_histone_assess/main.nf:30:17`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          bash "${projectDir}/bin/build.sh"
                  ^^^^^^^^^^
  ```

- Warning: `modules/local/distfit_histone_assess/main.nf:31:31`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH="\$PATH:${projectDir}/bin/HMM/build"
                                ^^^^^^^^^^
  ```

- Warning: `modules/local/distfit_histone_train/main.nf:10:30`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/src:${projectDir}/bin/HMM/build;
                               ^^^^^^^^^^
  ```

- Warning: `modules/local/distfit_histone_train/main.nf:10:52`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/src:${projectDir}/bin/HMM/build;
                                                     ^^^^^^^^^^
  ```

- Warning: `modules/local/distfit_histone_train/main.nf:11:51`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PYTHONPATH=\$PYTHONPATH:/app/src:${projectDir}/bin/src
                                                    ^^^^^^^^^^
  ```

- Warning: `modules/local/distfit_histone_train/main.nf:30:17`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          bash "${projectDir}/bin/build.sh"
                  ^^^^^^^^^^
  ```

- Warning: `modules/local/dm_decode/main.nf:10:30`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/src:${projectDir}/bin/HMM/build
                               ^^^^^^^^^^
  ```

- Warning: `modules/local/dm_decode/main.nf:10:52`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/src:${projectDir}/bin/HMM/build
                                                     ^^^^^^^^^^
  ```

- Warning: `modules/local/dm_decode/main.nf:11:51`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PYTHONPATH=\$PYTHONPATH:/app/src:${projectDir}/bin/src
                                                    ^^^^^^^^^^
  ```

- Warning: `modules/local/dm_decode/main.nf:31:17`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          bash "${projectDir}/bin/build.sh"
                  ^^^^^^^^^^
  ```

- Warning: `modules/local/dm_decode/main.nf:32:31`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH="\$PATH:${projectDir}/bin/HMM/build"
                                ^^^^^^^^^^
  ```

- Warning: `modules/local/dm_prepare/main.nf:10:30`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/src;
                               ^^^^^^^^^^
  ```

- Warning: `modules/local/dm_prepare/main.nf:11:51`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PYTHONPATH=\$PYTHONPATH:/app/src:${projectDir}/bin/src
                                                    ^^^^^^^^^^
  ```

- Warning: `modules/local/dm_report/main.nf:10:30`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/workflowTopology:${projectDir}/bin/src
                               ^^^^^^^^^^
  ```

- Warning: `modules/local/dm_report/main.nf:10:65`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/workflowTopology:${projectDir}/bin/src
                                                                  ^^^^^^^^^^
  ```

- Warning: `modules/local/dm_report/main.nf:11:51`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PYTHONPATH=\$PYTHONPATH:/app/src:${projectDir}/bin/src
                                                    ^^^^^^^^^^
  ```

- Warning: `modules/local/dm_train/main.nf:10:30`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/src:${projectDir}/bin/HMM/build
                               ^^^^^^^^^^
  ```

- Warning: `modules/local/dm_train/main.nf:10:52`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/src:${projectDir}/bin/HMM/build
                                                     ^^^^^^^^^^
  ```

- Warning: `modules/local/dm_train/main.nf:11:51`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PYTHONPATH=\$PYTHONPATH:/app/src:${projectDir}/bin/src
                                                    ^^^^^^^^^^
  ```

- Warning: `modules/local/dm_train/main.nf:34:17`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          bash "${projectDir}/bin/build.sh"
                  ^^^^^^^^^^
  ```

- Warning: `modules/local/dm_train/main.nf:35:31`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH="\$PATH:${projectDir}/bin/HMM/build"
                                ^^^^^^^^^^
  ```

- Warning: `modules/local/dna_decode/main.nf:10:30`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/src:${projectDir}/bin/HMM/build;
                               ^^^^^^^^^^
  ```

- Warning: `modules/local/dna_decode/main.nf:10:52`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/src:${projectDir}/bin/HMM/build;
                                                     ^^^^^^^^^^
  ```

- Warning: `modules/local/dna_decode/main.nf:11:51`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PYTHONPATH=\$PYTHONPATH:/app/src:${projectDir}/bin/src
                                                    ^^^^^^^^^^
  ```

- Warning: `modules/local/dna_decode/main.nf:29:17`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          bash "${projectDir}/bin/build.sh"
                  ^^^^^^^^^^
  ```

- Warning: `modules/local/dna_prepare/main.nf:10:30`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/src;
                               ^^^^^^^^^^
  ```

- Warning: `modules/local/dna_prepare/main.nf:11:51`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PYTHONPATH=\$PYTHONPATH:/app/src:${projectDir}/bin/src
                                                    ^^^^^^^^^^
  ```

- Warning: `modules/local/dna_report/main.nf:10:30`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/workflowDNAMethylation:${projectDir}/bin/src
                               ^^^^^^^^^^
  ```

- Warning: `modules/local/dna_report/main.nf:10:71`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/workflowDNAMethylation:${projectDir}/bin/src
                                                                        ^^^^^^^^^^
  ```

- Warning: `modules/local/dna_report/main.nf:11:51`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PYTHONPATH=\$PYTHONPATH:/app/src:${projectDir}/bin/src
                                                    ^^^^^^^^^^
  ```

- Warning: `modules/local/dna_train/main.nf:10:30`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/src:${projectDir}/bin/HMM/build;
                               ^^^^^^^^^^
  ```

- Warning: `modules/local/dna_train/main.nf:10:52`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/src:${projectDir}/bin/HMM/build;
                                                     ^^^^^^^^^^
  ```

- Warning: `modules/local/dna_train/main.nf:11:51`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PYTHONPATH=\$PYTHONPATH:/app/src:${projectDir}/bin/src
                                                    ^^^^^^^^^^
  ```

- Warning: `modules/local/dna_train/main.nf:29:17`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          bash "${projectDir}/bin/build.sh"
                  ^^^^^^^^^^
  ```

- Warning: `modules/local/dna_train/main.nf:30:31`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH="\$PATH:${projectDir}/bin/HMM/build"
                                ^^^^^^^^^^
  ```

- Warning: `modules/local/generate_methylation_bins/main.nf:28:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def wgbs_idx  = mods.findIndexOf { it == 'WGBS' }
                                         ^^
  ```

- Warning: `modules/local/std_decode/main.nf:10:30`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/src:${projectDir}/bin/HMM/build;
                               ^^^^^^^^^^
  ```

- Warning: `modules/local/std_decode/main.nf:10:52`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/src:${projectDir}/bin/HMM/build;
                                                     ^^^^^^^^^^
  ```

- Warning: `modules/local/std_decode/main.nf:11:51`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PYTHONPATH=\$PYTHONPATH:/app/src:${projectDir}/bin/src
                                                    ^^^^^^^^^^
  ```

- Warning: `modules/local/std_decode/main.nf:29:17`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          bash "${projectDir}/bin/build.sh"
                  ^^^^^^^^^^
  ```

- Warning: `modules/local/std_prepare/main.nf:10:30`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/src;
                               ^^^^^^^^^^
  ```

- Warning: `modules/local/std_prepare/main.nf:11:51`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PYTHONPATH=\$PYTHONPATH:/app/src:${projectDir}/bin/src
                                                    ^^^^^^^^^^
  ```

- Warning: `modules/local/std_report/main.nf:10:30`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/workflow:${projectDir}/bin/src
                               ^^^^^^^^^^
  ```

- Warning: `modules/local/std_report/main.nf:10:57`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/workflow:${projectDir}/bin/src
                                                          ^^^^^^^^^^
  ```

- Warning: `modules/local/std_report/main.nf:11:51`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PYTHONPATH=\$PYTHONPATH:/app/src:${projectDir}/bin/src
                                                    ^^^^^^^^^^
  ```

- Warning: `modules/local/std_train/main.nf:10:30`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/src:${projectDir}/bin/HMM/build;
                               ^^^^^^^^^^
  ```

- Warning: `modules/local/std_train/main.nf:10:52`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PATH=\$PATH:${projectDir}/bin/src:${projectDir}/bin/HMM/build;
                                                     ^^^^^^^^^^
  ```

- Warning: `modules/local/std_train/main.nf:11:51`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          export PYTHONPATH=\$PYTHONPATH:/app/src:${projectDir}/bin/src
                                                    ^^^^^^^^^^
  ```

- Warning: `modules/local/std_train/main.nf:31:17`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          bash "${projectDir}/bin/build.sh"
                  ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/distribution_fitting/main.nf:12:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/distribution_fitting/main.nf:17:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it[1] }
                    ^^
  ```

- Warning: `subworkflows/local/distribution_fitting/main.nf:21:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def header = h.withReader { it.readLine() }
                                          ^^
  ```

- Warning: `subworkflows/local/distribution_fitting/main.nf:44:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, csv -> csv }
                 ^^^^
  ```

- Warning: `subworkflows/local/generate_bins/main.nf:10:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/merge_data/main.nf:13:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/model_training_dm/main.nf:12:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/model_training_dna/main.nf:12:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/model_training_std/main.nf:12:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:6:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/process_histones/main.nf:11:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/process_histones/main.nf:32:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def list_of_metas = inputs.collect { it[0] }
                                                   ^^
  ```

- Warning: `subworkflows/local/process_histones/main.nf:33:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def list_of_bams  = inputs.collect { it[1] }
                                                   ^^
  ```

- Warning: `subworkflows/local/process_histones/main.nf:34:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def list_of_bais  = inputs.collect { it[2] }
                                                   ^^
  ```

- Warning: `subworkflows/local/process_methyl/main.nf:9:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_epigenomesegmentation_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_epigenomesegmentation_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:39:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_counts        = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:115:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_model_input = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:144:21`: Variable was declared but not used

  ```nextflow
                  def id             = tuple[0]
                      ^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:159:93`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def dist_list = params.distributions ? params.distributions.split(',').collect{ it.trim() } : []
                                                                                              ^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:164:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  Channel.fromPath(params.input).first()
                  ^^^^^^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:193:29`: Variable was declared but not used

  ```nextflow
                          def id             = tuple[0]
                              ^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:230:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:259:17`: Variable was declared but not used

  ```nextflow
          ).set { ch_collated_versions }
                  ^^^^^^^^^^^^^^^^^^^^
  ```
