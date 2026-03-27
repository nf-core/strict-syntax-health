# Nextflow lint results

- Generated: 2026-03-27T00:25:23.479321128Z
- Nextflow version: 26.03.1-edge
- Summary: 20 errors, 51 warnings

## :x: Errors

- Error: `modules/local/collect_stats.nf:24:5`: Invalid process output

  ```nextflow
      def score_threshold = params.mhcflurry_mhcnuggets_score_threshold
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `modules/local/collect_stats.nf:34:41`: `score_threshold` is not defined

  ```nextflow
                      --binder_threshold "$score_threshold"               \\
                                          ^^^^^^^^^^^^^^^^
  ```

- Error: `modules/local/download_proteins.nf:27:9`: `microbiome_ids` is already declared

  ```nextflow
      def microbiome_ids = microbiome_ids.join(' ')
          ^^^^^^^^^^^^^^
  ```

- Error: `modules/local/mhcflurry/main.nf:11:5`: Invalid process directive

  ```nextflow
      containerOptions = (workflow.containerEngine == 'docker') ? '-u $(id -u) -e "HOME=${HOME}" -v /etc/passwd:/etc/passwd:ro -v /etc/shadow:/etc/shadow:ro -v /etc/group:/etc/group:ro -v $HOME:$HOME' : ''
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `nextflow.config:201:35`: Invalid include source: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/metapep/conf/test_mhcnuggets_1.config'

  ```nextflow
      test_mhcnuggets_1           { includeConfig 'conf/test_mhcnuggets_1.config'             }
                                    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `nextflow.config:327:31`: `manifest` is not defined

  ```nextflow
  \033[0;35m  nf-core/metapep ${manifest.version}\033[0m
                                ^^^^^^^^
  ```

- Error: `nextflow.config:330:26`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                           ^^^^^^^^
  ```

- Error: `nextflow.config:330:69`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                      ^^^^^^^^
  ```

- Error: `nextflow.config:330:186`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                                                                                                                                           ^^^^^^^^
  ```

- Error: `nextflow.config:339:22`: `validation` is not defined

  ```nextflow
          beforeText = validation.help.beforeText
                       ^^^^^^^^^^
  ```

- Error: `nextflow.config:340:21`: `validation` is not defined

  ```nextflow
          afterText = validation.help.afterText
                      ^^^^^^^^^^
  ```

- Error: `subworkflows/local/mhc_binding_prediction/main.nf:112:5`: `valid_tools` was assigned but not declared

  ```nextflow
      valid_tools = [ 'mhcnuggets', 'mhcnuggetsii', 'mhcflurry', 'netmhcpan', 'netmhciipan' ]
      ^^^^^^^^^^^
  ```

- Error: `subworkflows/local/mhc_binding_prediction/main.nf:113:5`: `tool_list` was assigned but not declared

  ```nextflow
      tool_list = tools.tokenize(',')
      ^^^^^^^^^
  ```

- Error: `subworkflows/local/mhc_binding_prediction/main.nf:115:25`: `tool_list` is not defined

  ```nextflow
      def invalid_tools = tool_list.findAll { it.trim() !in valid_tools }
                          ^^^^^^^^^
  ```

- Error: `subworkflows/local/mhc_binding_prediction/main.nf:115:59`: `valid_tools` is not defined

  ```nextflow
      def invalid_tools = tool_list.findAll { it.trim() !in valid_tools }
                                                            ^^^^^^^^^^^
  ```

- Error: `subworkflows/local/mhc_binding_prediction/main.nf:117:110`: `valid_tools` is not defined

  ```nextflow
          throw new IllegalArgumentException("Invalid tools found: ${invalid_tools.join(',')}.\nValid tools: ${valid_tools.join(',')}")
                                                                                                               ^^^^^^^^^^^
  ```

- Error: `subworkflows/local/mhc_binding_prediction/main.nf:137:5`: `ch_netmhc_exe` was assigned but not declared

  ```nextflow
      ch_netmhc_exe = Channel.empty()
      ^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/mhc_binding_prediction/main.nf:138:5`: `ch_netmhc_exe` is not defined

  ```nextflow
      ch_netmhc_exe.bind([
      ^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/mhc_binding_prediction/main.nf:147:12`: `ch_netmhc_exe` is not defined

  ```nextflow
      return ch_netmhc_exe
             ^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/process_input.nf:118:103`: `microbiome_id` is not defined

  ```nextflow
                      if (bin_files.isEmpty()) log.warn("WARNING - Archive provided for microbiome ID ${microbiome_id} did not yield any bin files")
                                                                                                        ^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `modules/local/netmhciipan/main.nf:26:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          it.contains('DRB') ?
                          ^^
  ```

- Warning: `modules/local/netmhciipan/main.nf:27:29`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                              it.replace('*', '_').replace(':', '').replace('HLA-', '') :
                              ^^
  ```

- Warning: `modules/local/netmhciipan/main.nf:28:29`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                              it.replace('*', '').replace(':', '').replace('/','-').replace('H2','H-2')
                              ^^
  ```

- Warning: `modules/local/netmhciipan/main.nf:47:9`: Variable was declared but not used

  ```nextflow
      def args       = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/netmhcpan/main.nf:23:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def alleles = meta.alleles_supported.tokenize(';').collect { it.replace('*', '').replace('H2','H-2') }.join(',')
                                                                   ^^
  ```

- Warning: `modules/local/netmhcpan/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/prepare_prediction_input/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args       = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `nextflow.config:330:129`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                                                                                  ^^
  ```

- Warning: `subworkflows/local/mhc_binding_prediction/main.nf:32:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_versions = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/mhc_binding_prediction/main.nf:33:37`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_binding_predictors_out = Channel.empty()
                                      ^^^^^^^
  ```

- Warning: `subworkflows/local/mhc_binding_prediction/main.nf:92:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, file -> [meta.findAll { k, v -> k != 'alleles_supported' }, file] } // drop alleles_supported from meta
                                                  ^
  ```

- Warning: `subworkflows/local/mhc_binding_prediction/main.nf:115:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def invalid_tools = tool_list.findAll { it.trim() !in valid_tools }
                                              ^^
  ```

- Warning: `subworkflows/local/mhc_binding_prediction/main.nf:137:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_netmhc_exe = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/process_input.nf:15:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/process_input.nf:22:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      peptide_lengths = Channel.fromList( params.min_pep_len..params.max_pep_len )
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/process_input.nf:84:78`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      def bin_files = row.microbiome_path.listFiles().findAll{ it.name =~ fasta_suffix }
                                                                               ^^
  ```

- Warning: `subworkflows/local/process_input.nf:88:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          meta.bin_basename = it.name - fasta_suffix
                                              ^^
  ```

- Warning: `subworkflows/local/process_input.nf:89:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          return [ meta, it ]
                                         ^^
  ```

- Warning: `subworkflows/local/process_input.nf:114:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_bins_archives_input = Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/process_input.nf:117:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      bin_files = bin_files.findAll{ it.name =~ fasta_suffix }
                                                     ^^
  ```

- Warning: `subworkflows/local/process_input.nf:122:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          meta_new.bin_basename = it.name - fasta_suffix
                                                  ^^
  ```

- Warning: `subworkflows/local/process_input.nf:123:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          return [ meta_new, it ]
                                             ^^
  ```

- Warning: `subworkflows/local/process_input.nf:136:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_weights = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_metapep_pipeline/main.nf:31:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_metapep_pipeline/main.nf:38:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_metapep_pipeline/main.nf:69:53`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_samplesheet = params.show_supported_models ? Channel.empty() : Channel.fromPath(input, checkIfExists: true)
                                                      ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_metapep_pipeline/main.nf:69:71`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_samplesheet = params.show_supported_models ? Channel.empty() : Channel.fromPath(input, checkIfExists: true)
                                                                        ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:101:98`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      return ch_versions.unique().map { version -> processVersionsFromYAML(version) }.unique().mix(Channel.of(workflowVersionToYAML()))
                                                                                                   ^^^^^^^
  ```

- Warning: `workflows/metapep.nf:52:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/metapep.nf:53:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `workflows/metapep.nf:63:52`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_supported_alleles_and_peptide_lengths = Channel.fromPath(
                                                     ^^^^^^^
  ```

- Warning: `workflows/metapep.nf:82:57`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              PROCESS_INPUT.out.ch_taxa_input.map { meta, file -> meta.id }.collect(),
                                                          ^^^^
  ```

- Warning: `workflows/metapep.nf:83:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              PROCESS_INPUT.out.ch_taxa_input.map { meta, file -> file }.collect()
                                                    ^^^^
  ```

- Warning: `workflows/metapep.nf:113:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              PROCESS_INPUT.out.ch_weights.map { meta, file -> meta.id }.collect().ifEmpty([]),
                                                       ^^^^
  ```

- Warning: `workflows/metapep.nf:114:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              PROCESS_INPUT.out.ch_weights.map { meta, file -> file }.collect().ifEmpty([])
                                                 ^^^^
  ```

- Warning: `workflows/metapep.nf:127:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_pred_proteins_sorted.collect { meta, file -> file }.ifEmpty([]),
                                                ^^^^
  ```

- Warning: `workflows/metapep.nf:128:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_pred_proteins_sorted.collect { meta, file -> meta }.ifEmpty([]),
                                                      ^^^^
  ```

- Warning: `workflows/metapep.nf:205:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { base, txt, tsv, header_info -> header_info != null }
                        ^^^^
  ```

- Warning: `workflows/metapep.nf:205:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { base, txt, tsv, header_info -> header_info != null }
                              ^^^
  ```

- Warning: `workflows/metapep.nf:205:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { base, txt, tsv, header_info -> header_info != null }
                                   ^^^
  ```

- Warning: `workflows/metapep.nf:206:26`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { base, txt, tsv, header_info ->
                           ^^^
  ```

- Warning: `workflows/metapep.nf:242:65`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .combine(MHC_BINDING_PREDICTION.out.predicted.map { meta, file -> file }.toSortedList().flatten())
                                                                  ^^^^
  ```

- Warning: `workflows/metapep.nf:262:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_merge_predictions_input.collect(sort: { it.baseName }),
                                                         ^^
  ```

- Warning: `workflows/metapep.nf:340:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_config        = Channel.fromPath(
                                 ^^^^^^^
  ```

- Warning: `workflows/metapep.nf:343:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.fromPath(params.multiqc_config, checkIfExists: true) :
          ^^^^^^^
  ```

- Warning: `workflows/metapep.nf:344:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.empty()
          ^^^^^^^
  ```

- Warning: `workflows/metapep.nf:346:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.fromPath(params.multiqc_logo, checkIfExists: true) :
          ^^^^^^^
  ```

- Warning: `workflows/metapep.nf:347:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.fromPath("$projectDir/assets/nf-core-metapep_logo_light.png")
          ^^^^^^^
  ```

- Warning: `workflows/metapep.nf:351:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_workflow_summary = Channel.value(paramsSummaryMultiqc(summary_params))
                            ^^^^^^^
  ```

- Warning: `workflows/metapep.nf:357:45`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_methods_description                = Channel.value(
                                              ^^^^^^^
  ```

- Warning: `workflows/metapep.nf:380:5`: Variable was declared but not used

  ```nextflow
      multiqc_report = MULTIQC.out.report.toList()
      ^^^^^^^^^^^^^^
  ```
