# Nextflow lint results

- Generated: 2026-06-24T00:36:06.016300339Z
- Nextflow version: 26.05.0-edge
- Summary: 133 warnings

## :warning: Warnings

- Warning: `main.nf:40:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/gt_biopax/main.nf:14:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()                                           // For collecting tool versions
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/gt_biopax/main.nf:24:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          module = Channel.empty()
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/gt_diamond/main.nf:18:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()                                           // For collecting tool versions
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/gt_diamond/main.nf:27:14`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{network_id, seeds_meta, seeds, network_meta, network ->
               ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/gt_domino/main.nf:18:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()                                           // For collecting tool versions
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/gt_domino/main.nf:35:14`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{network_id, seeds_meta, seeds, network_meta, network, slices ->
               ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/gt_firstneighbor/main.nf:14:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/gt_firstneighbor/main.nf:20:14`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{network_id, seeds_meta, seeds, network_meta, network ->
               ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/gt_networkperturbation/main.nf:17:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/gt_networkperturbation/main.nf:23:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              precomputed: it[2].size() > 0
                           ^^
  ```

- Warning: `subworkflows/local/gt_networkperturbation/main.nf:31:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{meta, network, perturbed_networks -> [meta + [n_perturbations: params.n_network_perturbations], network]}
                              ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/gt_networkperturbation/main.nf:33:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          .combine(Channel.of(0..(params.n_network_perturbations-1)))
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/gt_networkperturbation/main.nf:45:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_perturbed_networks.precomputed.map{ meta, network, perturbed_networks -> [meta, perturbed_networks] }
                                                       ^^^^^^^
  ```

- Warning: `subworkflows/local/gt_networkperturbation/main.nf:74:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{key, meta, perturbed_modules ->
                    ^^^^
  ```

- Warning: `subworkflows/local/gt_networkperturbation/main.nf:86:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .multiMap{module_id, meta, module, perturbed_modules ->
                    ^^^^^^^^^
  ```

- Warning: `subworkflows/local/gt_networkperturbation/main.nf:97:15`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta, path -> path }
                ^^^^
  ```

- Warning: `subworkflows/local/gt_networkperturbation/main.nf:106:15`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta, path -> path }
                ^^^^
  ```

- Warning: `subworkflows/local/gt_proximity/main.nf:14:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/gt_proximity/main.nf:21:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_sp: it[2].name == "NO_FILE"
                     ^^
  ```

- Warning: `subworkflows/local/gt_proximity/main.nf:27:63`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      SHORTEST_PATHS(ch_shortest_paths.no_sp.map{meta, network, sp -> [meta, network]})
                                                                ^^
  ```

- Warning: `subworkflows/local/gt_proximity/main.nf:39:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .multiMap{network_id, meta, module, network, sp ->
                    ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/gt_proximity/main.nf:55:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions = ch_versions
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/gt_robust/main.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/gt_robust/main.nf:25:14`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{network_id, seeds_meta, seeds, network_meta, network ->
               ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/gt_robust_bias_aware/main.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/gt_robust_bias_aware/main.nf:27:14`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{network_id, seeds_meta, seeds, network_meta, network ->
               ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/gt_rwr/main.nf:18:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()                                           // For collecting tool versions
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/gt_rwr/main.nf:27:14`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{network_id, seeds_meta, seeds, network_meta, network ->
               ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/gt_seedperturbation/main.nf:19:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/gt_seedperturbation/main.nf:57:14`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{seeds_id, network_id, meta, perturbed_module, perturbed_seeds ->
               ^^^^^^^^
  ```

- Warning: `subworkflows/local/gt_seedperturbation/main.nf:57:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{seeds_id, network_id, meta, perturbed_module, perturbed_seeds ->
                         ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/gt_seedperturbation/main.nf:64:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{key, meta, perturbed_modules, perturbed_seeds ->
                    ^^^^
  ```

- Warning: `subworkflows/local/gt_seedperturbation/main.nf:75:14`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{seeds_id, network_id, meta, module, seeds -> [meta.module_id, meta, module, seeds]}
               ^^^^^^^^
  ```

- Warning: `subworkflows/local/gt_seedperturbation/main.nf:75:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{seeds_id, network_id, meta, module, seeds -> [meta.module_id, meta, module, seeds]}
                         ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/gt_seedperturbation/main.nf:83:14`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{module_id, meta, module, seeds, perturbed_modules, perturbed_seeds ->
               ^^^^^^^^^
  ```

- Warning: `subworkflows/local/gt_seedperturbation/main.nf:88:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .multiMap{network_id, meta, module, seeds, perturbed_modules, perturbed_seeds, network ->
                    ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/gt_seedperturbation/main.nf:107:15`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta, path -> path }
                ^^^^
  ```

- Warning: `subworkflows/local/gt_seedperturbation/main.nf:116:15`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta, path -> path }
                ^^^^
  ```

- Warning: `subworkflows/local/networkexpansion/main.nf:21:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      diamond_n = Channel.value(params.diamond_n)
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/networkexpansion/main.nf:22:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      diamond_alpha = Channel.value(params.diamond_alpha)
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/networkexpansion/main.nf:24:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      rwr_scaling = Channel.value(params.rwr_scaling).map{it ? 1 : 0}
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/networkexpansion/main.nf:24:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      rwr_scaling = Channel.value(params.rwr_scaling).map{it ? 1 : 0}
                                                          ^^
  ```

- Warning: `subworkflows/local/networkexpansion/main.nf:25:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      rwr_symmetrical = Channel.value(params.rwr_symmetrical).map{it ? 1 : 0}
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/networkexpansion/main.nf:25:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      rwr_symmetrical = Channel.value(params.rwr_symmetrical).map{it ? 1 : 0}
                                                                  ^^
  ```

- Warning: `subworkflows/local/networkexpansion/main.nf:26:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      rwr_r = Channel.value(params.rwr_r)
              ^^^^^^^
  ```

- Warning: `subworkflows/local/networkexpansion/main.nf:28:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      id_space = Channel.value(params.id_space)
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/networkexpansion/main.nf:31:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/networkexpansion/main.nf:32:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_modules  = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/networkexpansion/main.nf:33:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_raw_modules = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/networkexpansion/main.nf:76:14`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{seeds_id, network_id, meta, module, seeds ->
               ^^^^^^^^
  ```

- Warning: `subworkflows/local/networkexpansion/main.nf:76:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{seeds_id, network_id, meta, module, seeds ->
                         ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/networkexpansion/main.nf:86:14`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{network_id, meta, module, seeds, network ->
               ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:101:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_seeds = Channel.empty()          // channel: [ val(meta[id,seeds_id,network_id]), path(seeds) ]
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:102:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_network = Channel.empty()        // channel: [ val(meta[id,network_id]), path(network) ]
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:103:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_shortest_paths = Channel.empty() // channel: [ val(meta[id,network_id]), path(shortest_paths) ]
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:104:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_perturbed_networks = Channel.empty() // channel: [ val(meta[id,network_id]), [path(perturbed_network)] ]
                              ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:113:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_network = Channel.fromList(params.network.split(',').flatten())
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:125:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_input = Channel
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:182:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_seeds = Channel
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:184:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .combine(ch_network.map{meta, network, sp, perturbed_networks -> meta.network_id})
                                                ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:184:56`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .combine(ch_network.map{meta, network, sp, perturbed_networks -> meta.network_id})
                                                         ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:184:60`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .combine(ch_network.map{meta, network, sp, perturbed_networks -> meta.network_id})
                                                             ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:195:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .combine(ch_network.map{meta, network -> meta.network_id})
                                                ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:203:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                      Channel
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:213:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                      Channel
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:227:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_seeds = Channel
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:229:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .combine(ch_network.map{meta, network -> meta.network_id})
                                            ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:237:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  Channel
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:247:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  Channel
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:259:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_network.map{ meta, network, sp, perturbed_networks -> [meta.id] }
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:259:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_network.map{ meta, network, sp, perturbed_networks -> [meta.id] }
                                     ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:259:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_network.map{ meta, network, sp, perturbed_networks -> [meta.id] }
                                         ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:265:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_seeds.map{ meta, seeds -> [meta.id] }
                          ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:273:46`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_shortest_paths = ch_network.map{meta, network, sp, perturbed_networks ->
                                               ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:273:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_shortest_paths = ch_network.map{meta, network, sp, perturbed_networks ->
                                                            ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:277:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_perturbed_networks = ch_network.map{meta, network, sp, perturbed_networks ->
                                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:277:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_perturbed_networks = ch_network.map{meta, network, sp, perturbed_networks ->
                                                            ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:281:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_network = ch_network.map{meta, network, sp, perturbed_networks -> [meta, network]}
                                                 ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:281:52`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_network = ch_network.map{meta, network, sp, perturbed_networks -> [meta, network]}
                                                     ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:528:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def seeds_empty_count = seeds_empty.count  { key, value -> value == true }
                                                   ^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:529:52`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def module_empty_count = module_empty.count  { key, value -> value == true }
                                                     ^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:530:70`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def visualization_skipped_count = visualization_skipped.count  { key, value -> value == true }
                                                                       ^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_diseasemodulediscovery_pipeline/main.nf:531:62`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def drugstone_skipped_count = drugstone_skipped.count  { key, value -> value == true }
                                                               ^^^
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

- Warning: `workflows/diseasemodulediscovery.nf:126:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      id_space = Channel.value(params.id_space)
                 ^^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:127:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      validate_online = Channel.value(params.validate_online)
                        ^^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:134:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:135:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:136:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_seeds_empty_status = Channel.empty()
                              ^^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:137:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_module_empty_status = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:138:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_visualization_skipped_status = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:139:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_drugstone_skipped_status = Channel.empty()
                                    ^^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:145:15`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta, path -> path }
                ^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:160:14`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{key, meta, seeds, network -> [meta, seeds, network]}
               ^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:165:15`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta, path -> path }
                ^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:176:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{meta, seeds, network -> meta.id}
                     ^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:176:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{meta, seeds, network -> meta.id}
                            ^^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:208:15`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta, path -> path }
                ^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:234:14`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{newtork_id, meta, module, network -> [meta, module, network]}
               ^^^^^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:244:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter{meta, module -> meta.nodes > 0} // Filter out empty modules
                        ^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:250:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch{ meta, module ->
                         ^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:258:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .mix(ch_modules_empty_not_empty.empty.map {meta, module -> [meta.id, true] })
                                                           ^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:259:62`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .mix(ch_modules_empty_not_empty.not_empty.map {meta, module -> [meta.id, false] })
                                                               ^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:264:21`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map {meta, module -> "$meta.id\t$meta.nodes" }
                      ^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:282:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch {meta, module ->
                             ^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:289:57`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .mix(ch_visualization_input.fail.map {meta, module -> [meta.id, true] })
                                                          ^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:290:57`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .mix(ch_visualization_input.pass.map {meta, module -> [meta.id, false] })
                                                          ^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:295:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map {meta, module -> "$meta.id\t$meta.nodes" }
                          ^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:315:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch {meta, module ->
                             ^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:322:56`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .mix(ch_drugstone_export_input.fail.map {meta, module -> [meta.id, true] })
                                                         ^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:323:56`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .mix(ch_drugstone_export_input.pass.map {meta, module -> [meta.id, false] })
                                                         ^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:328:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map {meta, module -> "$meta.id\t$meta.nodes" }
                          ^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:344:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map{ meta, path -> path }
                    ^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:398:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .multiMap{key, meta, nodes, network ->
                            ^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:420:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .multiMap{key, meta, nodes, network ->
                            ^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:429:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      .map{ meta, path -> path }
                            ^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:442:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      .filter{ meta, nodes -> meta.amim != "no_tool" } // Filter out no_tool modules
                                     ^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:445:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      .multiMap{key, meta, nodes, network ->
                                ^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:454:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      .map{ meta, path -> path }
                            ^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:480:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ch_modules.filter{ meta, path -> meta.amim != "no_tool" }, // Filter out no_tool modules
                                           ^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:493:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ch_modules.filter{ meta, path -> meta.amim != "no_tool" }, // Filter out no_tool modules
                                           ^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:517:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_algorithms_drugs = Channel
                                ^^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:527:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch {meta, module ->
                             ^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:541:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          includeIndirectDrugs = Channel.value(params.includeIndirectDrugs).map{it ? 1 : 0}
                                 ^^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:541:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          includeIndirectDrugs = Channel.value(params.includeIndirectDrugs).map{it ? 1 : 0}
                                                                                ^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:542:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          includeNonApprovedDrugs = Channel.value(params.includeNonApprovedDrugs).map{it ? 1 : 0}
                                    ^^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:542:85`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          includeNonApprovedDrugs = Channel.value(params.includeNonApprovedDrugs).map{it ? 1 : 0}
                                                                                      ^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:549:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .map{ meta, algorithm, drug_predictions -> [meta, drug_predictions] }
                              ^^^^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:550:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .filter{ meta, drug_predictions -> meta.nodes <= params.visualization_max_nodes }       // Filter out modules with too many nodes
                                 ^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/diseasemodulediscovery.nf:553:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .map{module_id, meta, drug_predictions, module -> [meta, module, drug_predictions] }    // Format for visualization
                       ^^^^^^^^^
  ```
