# Nextflow lint results

- Generated: 2026-05-14T00:37:26.062945354Z
- Nextflow version: 26.04.1
- Summary: 104 warnings

## :warning: Warnings

- Warning: `main.nf:277:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          path { name, meta, file ->
                             ^^^^
  ```

- Warning: `main.nf:310:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          path { name, meta, file ->
                             ^^^^
  ```

- Warning: `main.nf:327:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          path { name, meta, file ->
                             ^^^^
  ```

- Warning: `main.nf:378:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          path { name, meta, file ->
                             ^^^^
  ```

- Warning: `main.nf:387:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          path { name, meta, file ->
                 ^^^^
  ```

- Warning: `main.nf:387:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          path { name, meta, file ->
                             ^^^^
  ```

- Warning: `main.nf:392:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          path { name, meta, file ->
                 ^^^^
  ```

- Warning: `main.nf:392:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          path { name, meta, file ->
                             ^^^^
  ```

- Warning: `main.nf:397:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          path { name, meta, file ->
                 ^^^^
  ```

- Warning: `main.nf:397:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          path { name, meta, file ->
                       ^^^^
  ```

- Warning: `main.nf:397:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          path { name, meta, file ->
                             ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_differentialabundance_pipeline/main.nf:29:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      validate_params   // boolean: Boolean whether to validate parameters against the schema at runtime
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_differentialabundance_pipeline/main.nf:33:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_differentialabundance_pipeline/main.nf:40:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_differentialabundance_pipeline/main.nf:105:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_paramsets = Channel.fromList(paramsets)
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_differentialabundance_pipeline/main.nf:109:41`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              params: paramset.findAll{ k,v -> k != 'paramset_name' }
                                          ^
  ```

- Warning: `subworkflows/local/utils_nfcore_differentialabundance_pipeline/main.nf:405:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          def cleanparamset = paramset.findAll { k, v -> !(ignore + nonstaticparams).contains(k) } as Map
                                                    ^
  ```

- Warning: `subworkflows/local/utils_nfcore_differentialabundance_pipeline/main.nf:409:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          def notnullparams = cleanparamset.findAll { k, v -> v != null } as Map
                                                      ^
  ```

- Warning: `subworkflows/local/utils_nfcore_differentialabundance_pipeline/main.nf:414:18`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          } catch (e) {
                   ^
  ```

- Warning: `subworkflows/local/utils_nfcore_differentialabundance_pipeline/main.nf:498:9`: Variable was declared but not used

  ```nextflow
      def yaml_parser = new org.yaml.snakeyaml.Yaml()
          ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_differentialabundance_pipeline/main.nf:515:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def includedConfig = includeConfigs.find { it.paramset_name == paramsetName }
                                                         ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_differentialabundance_pipeline/main.nf:544:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def simplifiedparams = getRelevantParams(it[0].params, category)
                                                       ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_differentialabundance_pipeline/main.nf:546:34`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def simplifiedmeta = it[0] + [params: simplifiedparams]
                                   ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_differentialabundance_pipeline/main.nf:550:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              def key = simplifiedmeta.findAll { k, v -> k != 'paramset_name' }
                                                    ^
  ```

- Warning: `subworkflows/local/utils_nfcore_differentialabundance_pipeline/main.nf:551:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              [key, it[1..-1]]  // [ key, [files] ]
                    ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_differentialabundance_pipeline/main.nf:585:76`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              def meta_cleaned = meta_keys_to_remove ? meta_out.findAll { k, v -> !meta_keys_to_remove.contains(k) } : meta_out
                                                                             ^
  ```

- Warning: `subworkflows/local/utils_nfcore_differentialabundance_pipeline/main.nf:634:67`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          def matchingGroups = schema['$defs'].findAll { groupName, group ->
                                                                    ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_differentialabundance_pipeline/main.nf:638:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          matchingGroups.each { groupName, group ->
                                ^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_differentialabundance_pipeline/main.nf:640:52`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  group.properties.each { paramName, paramProps ->
                                                     ^^^^^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:69:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, input ->
                          ^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:78:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, input ->
                       ^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:90:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, input ->
                       ^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:110:109`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  [ meta, meta.params.gene_sets_files ? meta.params.gene_sets_files.split(",").collect { file(it, checkIfExists: true) } : [] ]
                                                                                                              ^^
  ```

- Warning: `workflows/differentialabundance.nf:130:18`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch{ meta, file, extension ->
                   ^^^^
  ```

- Warning: `workflows/differentialabundance.nf:130:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch{ meta, file, extension ->
                         ^^^^
  ```

- Warning: `workflows/differentialabundance.nf:137:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .flatMap { meta, yaml_file, ext ->
                                      ^^^
  ```

- Warning: `workflows/differentialabundance.nf:148:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter { it != null }
                        ^^
  ```

- Warning: `workflows/differentialabundance.nf:153:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, row, ext ->
                            ^^^
  ```

- Warning: `workflows/differentialabundance.nf:250:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{meta, input -> [meta, file(meta.params.matrix, checkIfExists: true)]}
                     ^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:267:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              user_features: it.params.features
                             ^^
  ```

- Warning: `workflows/differentialabundance.nf:268:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              affy_features: it.params.study_type == 'affy_array'
                             ^^
  ```

- Warning: `workflows/differentialabundance.nf:269:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              geo_features: it.params.study_type == 'geo_soft_file'
                            ^^
  ```

- Warning: `workflows/differentialabundance.nf:270:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              gtf_features: it.params.gtf
                            ^^
  ```

- Warning: `workflows/differentialabundance.nf:293:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              compressed: it[1].name.endsWith('.gz')
                          ^^
  ```

- Warning: `workflows/differentialabundance.nf:294:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              uncompressed: !it[1].name.endsWith('.gz')
                             ^^
  ```

- Warning: `workflows/differentialabundance.nf:354:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map{tuple(it[0], [it[1], it[2]])}
                     ^^
  ```

- Warning: `workflows/differentialabundance.nf:354:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map{tuple(it[0], [it[1], it[2]])}
                             ^^
  ```

- Warning: `workflows/differentialabundance.nf:354:35`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map{tuple(it[0], [it[1], it[2]])}
                                    ^^
  ```

- Warning: `workflows/differentialabundance.nf:388:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter{meta, assays -> meta.params.study_type == 'affy_array' || meta.params.study_type == 'maxquant'}
                        ^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:390:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, assay ->
                    ^^^^
  ```

- Warning: `workflows/differentialabundance.nf:398:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .mix(ch_validated_assays.filter{meta, assay -> meta.params.study_type in ['rnaseq', 'generic_matrix']})
                                                ^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:406:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .mix(ch_validated_assays.filter{meta, assay -> meta.params.study_type in ['rnaseq', 'generic_matrix'] || meta.params.study_type == 'geo_soft_file'})
                                                ^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:511:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta_key, meta_with_contrast, results_file, features_file ->
                 ^^^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:527:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter{meta, matrix -> meta.params.study_type in ['rnaseq', 'generic_matrix']}
                        ^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:529:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .mix(ch_validated_assays.filter{meta, assay -> meta.params.study_type == 'geo_soft_file'})
                                                ^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:550:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter{meta, matrix -> meta.params.functional_method == 'gprofiler2' && meta.params.gprofiler2_background_file == "auto"}
                        ^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:567:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter{meta, matrix -> meta.params.functional_method == 'gsea'}
                        ^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:574:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .filter{meta, meta_with_contrast, results -> meta.params.functional_method == 'gprofiler2'}
                                ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:574:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .filter{meta, meta_with_contrast, results -> meta.params.functional_method == 'gprofiler2'}
                                                    ^^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:579:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .filter{meta, meta_with_contrast, results -> meta.params.functional_method == 'decoupler'}
                                ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:579:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .filter{meta, meta_with_contrast, results -> meta.params.functional_method == 'decoupler'}
                                                    ^^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:588:16`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { it.tail() } // remove the meta without contrast info that is used as key
                 ^^
  ```

- Warning: `workflows/differentialabundance.nf:634:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_mat = ch_norm.filter{meta, matrix -> meta.params.study_type == 'geo_soft_file'}
                                    ^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:638:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .filter{meta, raw -> meta.params.study_type != 'geo_soft_file'}
                                ^^^
  ```

- Warning: `workflows/differentialabundance.nf:672:14`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map{it.tail()}  // remove the meta without contrast info that is used as key
               ^^
  ```

- Warning: `workflows/differentialabundance.nf:709:61`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, meta_with_contrast, results, contrast, variable, reference, target, formula, comparison ->
                                                              ^^^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:709:71`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, meta_with_contrast, results, contrast, variable, reference, target, formula, comparison ->
                                                                        ^^^^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:709:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, meta_with_contrast, results, contrast, variable, reference, target, formula, comparison ->
                                                                                   ^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:709:90`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, meta_with_contrast, results, contrast, variable, reference, target, formula, comparison ->
                                                                                           ^^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:709:99`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, meta_with_contrast, results, contrast, variable, reference, target, formula, comparison ->
                                                                                                    ^^^^^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:713:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def contrast_maps = meta_with_contrast.collect { it.subMap(paramset_contrast_keys) }
                                                               ^^
  ```

- Warning: `workflows/differentialabundance.nf:725:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def content = contrast_map.collect { it.values().join(',') }.sort().reverse()
                                                   ^^
  ```

- Warning: `workflows/differentialabundance.nf:730:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [it.baseName, it] }
                  ^^
  ```

- Warning: `workflows/differentialabundance.nf:730:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [it.baseName, it] }
                               ^^
  ```

- Warning: `workflows/differentialabundance.nf:731:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .join( ch_paramsets.map { [it.paramset_name, it] } )
                                     ^^
  ```

- Warning: `workflows/differentialabundance.nf:731:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .join( ch_paramsets.map { [it.paramset_name, it] } )
                                                       ^^
  ```

- Warning: `workflows/differentialabundance.nf:732:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { paramset_name, contrast_file, meta ->
                 ^^^^^^^^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:739:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, contrast, results -> contrast.variable?.trim() }
                    ^^^^
  ```

- Warning: `workflows/differentialabundance.nf:739:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, contrast, results -> contrast.variable?.trim() }
                                    ^^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:742:61`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, meta_with_contrast, results, contrast, variable, reference, target, formula, comparison ->
                                                              ^^^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:742:71`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, meta_with_contrast, results, contrast, variable, reference, target, formula, comparison ->
                                                                        ^^^^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:742:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, meta_with_contrast, results, contrast, variable, reference, target, formula, comparison ->
                                                                                   ^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:742:90`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, meta_with_contrast, results, contrast, variable, reference, target, formula, comparison ->
                                                                                           ^^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:742:99`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, meta_with_contrast, results, contrast, variable, reference, target, formula, comparison ->
                                                                                                    ^^^^^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:744:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def contrast_maps = meta_with_contrast.collect { it.subMap(paramset_contrast_keys) }
                                                               ^^
  ```

- Warning: `workflows/differentialabundance.nf:756:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def content = contrast_map.collect { it.values().collect { val ->
                                                   ^^
  ```

- Warning: `workflows/differentialabundance.nf:762:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [it.baseName.replaceAll('_shinyngs$', ''), it] }
                  ^^
  ```

- Warning: `workflows/differentialabundance.nf:762:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [it.baseName.replaceAll('_shinyngs$', ''), it] }
                                                            ^^
  ```

- Warning: `workflows/differentialabundance.nf:763:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .join( ch_paramsets.map { [it.paramset_name, it] } )
                                     ^^
  ```

- Warning: `workflows/differentialabundance.nf:763:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .join( ch_paramsets.map { [it.paramset_name, it] } )
                                                       ^^
  ```

- Warning: `workflows/differentialabundance.nf:764:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { paramset_name, contrast_file, meta ->
                 ^^^^^^^^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:775:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .multiMap { meta, meta_with_contrast, differential_results, contrast_file, samplesheet, features, matrices ->
                            ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:778:96`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              contrast_stats_assay: meta.params.exploratory_assay_names.split(',').findIndexOf { it == meta.params.exploratory_final_assay } + 1
                                                                                                 ^^
  ```

- Warning: `workflows/differentialabundance.nf:793:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:845:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [it[0], it.tail().tail().flatten()] }  // [ meta, [differential results and models] ]
                  ^^
  ```

- Warning: `workflows/differentialabundance.nf:845:24`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [it[0], it.tail().tail().flatten()] }  // [ meta, [differential results and models] ]
                         ^^
  ```

- Warning: `workflows/differentialabundance.nf:849:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [it[0], it.tail().tail().flatten()] }  // [ meta, [functional results] ]
                  ^^
  ```

- Warning: `workflows/differentialabundance.nf:849:24`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [it[0], it.tail().tail().flatten()] }  // [ meta, [functional results] ]
                         ^^
  ```

- Warning: `workflows/differentialabundance.nf:862:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [it[0], it.tail().flatten().grep()] }  // [meta, [files]]   // note that grep() would remove null files from join with remainder true
                  ^^
  ```

- Warning: `workflows/differentialabundance.nf:862:24`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [it[0], it.tail().flatten().grep()] }  // [meta, [files]]   // note that grep() would remove null files from join with remainder true
                         ^^
  ```

- Warning: `workflows/differentialabundance.nf:864:26`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .flatMap { meta, report_file, files ->
                           ^^^^^^^^^^^
  ```

- Warning: `workflows/differentialabundance.nf:881:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  paramset.exploratory_assay_names.split(',').collect { "${it}_matrix".toString() } +
                                                                           ^^
  ```

- Warning: `workflows/differentialabundance.nf:896:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_report_input.input_files.map{ meta, files -> files },
                                           ^^^^
  ```

- Warning: `workflows/differentialabundance.nf:897:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.value([])
          ^^^^^^^
  ```
