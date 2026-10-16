# Nextflow lint results

- Generated: 2026-10-16T00:19:29.313685837Z
- Nextflow version: 26.10.1
- Summary: 127 warnings

## :warning: Warnings

- Warning: `modules/local/general_mergefile/main.nf:16:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/general_mergefile/main.nf:22:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def inputs        = input_target.collect { it }.join(' ')
                                                 ^^
  ```

- Warning: `modules/local/ms2query_checkmodelfiles/main.nf:26:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/ms2query_checkmodelfiles/main.nf:31:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def model_files        = modelfiles.collect { it }.join(' ')
                                                    ^^
  ```

- Warning: `modules/local/ms2query_downloadmodel/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/ms2query_modeltrain/main.nf:25:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/ms2query_modeltrain/main.nf:30:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/ms2query_search/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/openms_featurefindermetabo/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/openms_featurefindermetaboident/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/openms_featurelinkerunlabeledkd/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/openms_featurelinkerunlabeledkd/main.nf:23:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def featurexml_input        = featurexml.collect { it }.join(' ')
                                                         ^^
  ```

- Warning: `modules/local/openms_filefilter/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/openms_mapalignerposeclustering/main.nf:16:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      tuple val(meta), path({meta.id.collect { 'output/'+it+'.trafoXML' }}), emit: trafoxml
                                                         ^^
  ```

- Warning: `modules/local/openms_mapalignerposeclustering/main.nf:17:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      tuple val(meta), path({meta.id.collect { 'output/'+it+'.featureXML' }}), emit: featurexml
                                                         ^^
  ```

- Warning: `modules/local/openms_mapalignerposeclustering/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/openms_mapalignerposeclustering/main.nf:27:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def featurexml_input        = featurexml.collect { it }.join(' ')
                                                         ^^
  ```

- Warning: `modules/local/openms_mapalignerposeclustering/main.nf:28:61`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def trafoxml_output        = prefix.collect { 'output/'+it+'.trafoXML' }.join(' ')
                                                              ^^
  ```

- Warning: `modules/local/openms_mapalignerposeclustering/main.nf:29:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def featurexml_output        = prefix.collect { 'output/'+it+'.featureXML' }.join(' ')
                                                                ^^
  ```

- Warning: `modules/local/openms_mapalignerposeclusteringmzml/main.nf:14:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      tuple val(meta), path({meta.id.collect { 'output/'+it+'.trafoXML' }}), emit: trafoxml
                                                         ^^
  ```

- Warning: `modules/local/openms_mapalignerposeclusteringmzml/main.nf:15:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      tuple val(meta), path({meta.id.collect { 'output/'+it+'.mzML' }}), emit: mzml
                                                         ^^
  ```

- Warning: `modules/local/openms_mapalignerposeclusteringmzml/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/openms_mapalignerposeclusteringmzml/main.nf:26:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def featurexml_input        = featurexml.collect { it }.join(' ')
                                                         ^^
  ```

- Warning: `modules/local/openms_mapalignerposeclusteringmzml/main.nf:27:61`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def trafoxml_output        = prefix.collect { 'output/'+it+'.trafoXML' }.join(' ')
                                                              ^^
  ```

- Warning: `modules/local/openms_mapalignerposeclusteringmzml/main.nf:28:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def mzml_output        = prefix.collect { 'output/'+it+'.mzML' }.join(' ')
                                                          ^^
  ```

- Warning: `modules/local/openms_maprttransformer/main.nf:16:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/openms_metaboliteadductdecharger/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/openms_peakpickerhires/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pyopenms_c13detection/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pyopenms_calculateboundries/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pyopenms_conctsv/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pyopenms_conctsv/main.nf:25:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/pyopenms_export/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pyopenms_extractfeaturemz/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pyopenms_filemerger/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pyopenms_filemerger/main.nf:26:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def inputs        = consensusxml_input.collect { it }.join(' ')
                                                       ^^
  ```

- Warning: `modules/local/pyopenms_generatesearchparams/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pyopenms_generatesearchparams/main.nf:27:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def mzml_input        = input_spectra.collect { it }.join(' ')
                                                      ^^
  ```

- Warning: `modules/local/pyopenms_generatesearchparams/main.nf:28:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def csv_output        = input_spectra.collect { "output/${it.baseName}${map_index}.csv" }.join(' ')
                                                                ^^
  ```

- Warning: `modules/local/pyopenms_generatesearchparamsunmapped/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pyopenms_libbuilder/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pyopenms_merge/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pyopenms_msmapping/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pyopenms_msmapping/main.nf:24:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def mzml_input        = input_spectra.collect { it }.join(' ')
                                                      ^^
  ```

- Warning: `modules/local/pyopenms_reloadmaps/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pyopenms_split/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pyopenms_splitconsensus/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pyopenms_splitconsensus/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/pyopenms_splitfeaturexml/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pyopenms_splitfeaturexml/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/pyopenms_splitmgf/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pyopenms_splitmgf/main.nf:26:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/sirius_search/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/sirius_search/main.nf:24:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/multiqc/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `subworkflows/local/annotation/main.nf:9:9`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          empty_id
          ^^^^^^^^
  ```

- Warning: `subworkflows/local/annotation/main.nf:10:9`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          separate
          ^^^^^^^^
  ```

- Warning: `subworkflows/local/annotation/main.nf:11:9`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          mzml_files
          ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/annotation/main.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/annotation/main.nf:20:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          OPENMS_METABOLITEADDUCTDECHARGER(quantification_information.map{it[0,1]})
                                                                          ^^
  ```

- Warning: `subworkflows/local/annotation/main.nf:21:9`: Variable was declared but not used

  ```nextflow
          quantified_features=OPENMS_METABOLITEADDUCTDECHARGER.out.featurexml
          ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/annotation/main.nf:23:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .join(quantification_information.map{it[0,2]},by:[0])
                                               ^^
  ```

- Warning: `subworkflows/local/identification/main.nf:23:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      quantification_information
      ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/identification/main.nf:41:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  ch_versions = Channel.empty()
                ^^^^^^^
  ```

- Warning: `subworkflows/local/identification/main.nf:46:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
  consensusxml_data.combine(mzml_files.filter{meta,file->meta.level == "MS2" | meta.level == "MS12"}.collect{it[1]}
                                                   ^^^^
  ```

- Warning: `subworkflows/local/identification/main.nf:46:108`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  consensusxml_data.combine(mzml_files.filter{meta,file->meta.level == "MS2" | meta.level == "MS12"}.collect{it[1]}
                                                                                                             ^^
  ```

- Warning: `subworkflows/local/identification/main.nf:70:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  filtered_consensus = PYOPENMS_SPLITCONSENSUS.out.consensusxml.map{it[1]}.flatten().map{ file ->
                                                                    ^^
  ```

- Warning: `subworkflows/local/identification/main.nf:83:26`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
  mzml_files.filter{ meta, file -> meta.level == "MS2" || meta.level == "MS12" }.map{tuple ->
                           ^^^^
  ```

- Warning: `subworkflows/local/identification/main.nf:90:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def metas = sortedTuples.collect { it[0] }
                                             ^^
  ```

- Warning: `subworkflows/local/identification/main.nf:91:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def files = sortedTuples.collect { it[1] }
                                             ^^
  ```

- Warning: `subworkflows/local/identification/main.nf:98:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  csv_unmmaped_channel = PYOPENMS_GENERATESEARCHPARAMS.out.csv.map{it[1]}.flatten().map{file -> [[id:file.baseName],file]}
                                                                   ^^
  ```

- Warning: `subworkflows/local/identification/main.nf:99:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  ms_mmaped_channel = PYOPENMS_GENERATESEARCHPARAMS.out.ms.map{it[1]}.flatten().map{file -> [[id:file.baseName],file]}
                                                               ^^
  ```

- Warning: `subworkflows/local/identification/main.nf:100:64`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  mgf_mmaped_channel = PYOPENMS_GENERATESEARCHPARAMS.out.mgf.map{it[1]}.flatten().map{file -> [[id:file.baseName],file]}
                                                                 ^^
  ```

- Warning: `subworkflows/local/identification/main.nf:106:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  generated_params = OPENMS_FILEFILTER.out.consensusxml.map{it[0]}.combine(
                                                            ^^
  ```

- Warning: `subworkflows/local/identification/main.nf:107:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  PYOPENMS_GENERATESEARCHPARAMS.out.csv.collect{it[1]}
                                                ^^
  ```

- Warning: `subworkflows/local/identification/main.nf:123:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  }.toList()).map{it[1]}.flatten()
                  ^^
  ```

- Warning: `subworkflows/local/identification/main.nf:137:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  OPENMS_FILEFILTER.out.consensusxml.map{it[0]}.combine(
                                         ^^
  ```

- Warning: `subworkflows/local/identification/main.nf:138:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  PYOPENMS_GENERATESEARCHPARAMS.out.ms.collect{it[1]}
                                               ^^
  ```

- Warning: `subworkflows/local/identification/main.nf:154:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  }.toList()).map{it[1]}.flatten()
                  ^^
  ```

- Warning: `subworkflows/local/identification/main.nf:165:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  OPENMS_FILEFILTER.out.consensusxml.map{it[0]}.combine(
                                         ^^
  ```

- Warning: `subworkflows/local/identification/main.nf:166:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  PYOPENMS_GENERATESEARCHPARAMS.out.mgf.collect{it[1]}
                                                ^^
  ```

- Warning: `subworkflows/local/identification/main.nf:182:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  }.toList()).map{it[1]}.flatten()
                  ^^
  ```

- Warning: `subworkflows/local/identification/main.nf:198:26`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
  mzml_files.filter{ meta, file -> meta.level == "MS2" || meta.level == "MS12" }
                           ^^^^
  ```

- Warning: `subworkflows/local/identification/main.nf:201:7`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  ).map{it[1,2,3]} | PYOPENMS_GENERATESEARCHPARAMSUNMAPPED
        ^^
  ```

- Warning: `subworkflows/local/identification/main.nf:210:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  output_sirius = Channel.empty()
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/identification/main.nf:211:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  output_fingerid = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/identification/main.nf:226:12`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  ms2query = Channel.empty()
             ^^^^^^^
  ```

- Warning: `subworkflows/local/linker/main.nf:19:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_versions = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/linker/main.nf:25:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      quantification_information.map{it[0,1]} | PYOPENMS_EXTRACTFEATUREMZ
                                     ^^
  ```

- Warning: `subworkflows/local/linker/main.nf:31:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  PYOPENMS_CONCTSV_MZ(Channel.of([id:"merged_mz_range"]).combine(PYOPENMS_EXTRACTFEATUREMZ.out.tsv.collect{it[1]}.toList()),"tsv","tsv")
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/linker/main.nf:31:106`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  PYOPENMS_CONCTSV_MZ(Channel.of([id:"merged_mz_range"]).combine(PYOPENMS_EXTRACTFEATUREMZ.out.tsv.collect{it[1]}.toList()),"tsv","tsv")
                                                                                                           ^^
  ```

- Warning: `subworkflows/local/linker/main.nf:38:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  PYOPENMS_SPLITFEATUREXML(quantification_information.map{it[0,1]},
                                                          ^^
  ```

- Warning: `subworkflows/local/linker/main.nf:39:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      PYOPENMS_CALCULATEBOUNDRIES.out.tsv.map{it[1]}
                                              ^^
  ```

- Warning: `subworkflows/local/linker/main.nf:45:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  PYOPENMS_SPLITFEATUREXML.out.featurexml.collect{it[1]}.flatten().map{file ->
                                                  ^^
  ```

- Warning: `subworkflows/local/linker/main.nf:55:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  to_be_merged = Channel.of([id:"Linked_data"]).combine(
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/linker/main.nf:56:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  OPENMS_FEATURELINKERUNLABELEDKDPARTS.out.consensusxml.map{it[1]}.collect()
                                                            ^^
  ```

- Warning: `subworkflows/local/linker/main.nf:77:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
  consensusxml=   PYOPENMS_FILEMERGER.out.consensusxml.map{meta,consensus_file->[[id:consensus_file.baseName],consensus_file]}
                                                           ^^^^
  ```

- Warning: `subworkflows/local/linker/main.nf:81:1`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  Channel.of([id:"Linked_data"]).combine(quantification_information.collect{it[1]}.map { files ->
  ^^^^^^^
  ```

- Warning: `subworkflows/local/linker/main.nf:81:75`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  Channel.of([id:"Linked_data"]).combine(quantification_information.collect{it[1]}.map { files ->
                                                                            ^^
  ```

- Warning: `subworkflows/local/linker/main.nf:88:75`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          consensusxml=OPENMS_FEATURELINKERUNLABELEDKD.out.consensusxml.map{meta,consensus_file->[[id:consensus_file.baseName],consensus_file]}
                                                                            ^^^^
  ```

- Warning: `subworkflows/local/ms2query/main.nf:26:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  ch_versions = Channel.empty()
                ^^^^^^^
  ```

- Warning: `subworkflows/local/ms2query/main.nf:40:1`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  Channel
  ^^^^^^^
  ```

- Warning: `subworkflows/local/ms2query/main.nf:65:85`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  mgf_channel = PYOPENMS_SPLITMGF.out.mgf.flatMap{id, values -> values.collect { [id, it]}}
                                                                                      ^^
  ```

- Warning: `subworkflows/local/ms2query/main.nf:73:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `subworkflows/local/ms2query_modeldownloader/main.nf:8:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/ms2query_modeldownloader/main.nf:12:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `subworkflows/local/ms2query_modeldownloader/main.nf:18:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `subworkflows/local/quantification/main.nf:17:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/quantification/main.nf:28:24`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      mzml_files.collect{it[0]}.toList().combine(mzml_files.collect{it[1]}.toList()) | OPENMS_MAPALIGNERPOSECLUSTERINGMZML
                         ^^
  ```

- Warning: `subworkflows/local/quantification/main.nf:28:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      mzml_files.collect{it[0]}.toList().combine(mzml_files.collect{it[1]}.toList()) | OPENMS_MAPALIGNERPOSECLUSTERINGMZML
                                                                    ^^
  ```

- Warning: `subworkflows/local/quantification/main.nf:33:85`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      [[map_id:idd],meta,mzml]}.join(OPENMS_MAPALIGNERPOSECLUSTERINGMZML.out.mzml.map{it[1]}.flatten().map{mzml ->
                                                                                      ^^
  ```

- Warning: `subworkflows/local/quantification/main.nf:35:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      [[map_id:idd], mzml]}).map{it[1,3]}
                                 ^^
  ```

- Warning: `subworkflows/local/quantification/main.nf:44:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
  quantificaiton_data=mzml_files.filter{meta,file->meta.level == "MS1" | meta.level == "MS12"}
                                             ^^^^
  ```

- Warning: `subworkflows/local/quantification/main.nf:53:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      quantified_features.collect{it[0]}.toList().combine(quantified_features.collect{it[1]}.toList()) | OPENMS_MAPALIGNERPOSECLUSTERING
                                  ^^
  ```

- Warning: `subworkflows/local/quantification/main.nf:53:85`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      quantified_features.collect{it[0]}.toList().combine(quantified_features.collect{it[1]}.toList()) | OPENMS_MAPALIGNERPOSECLUSTERING
                                                                                      ^^
  ```

- Warning: `subworkflows/local/quantification/main.nf:59:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      .join(OPENMS_MAPALIGNERPOSECLUSTERING.out.featurexml.map{it[1]}.flatten().map{featurexml ->
                                                               ^^
  ```

- Warning: `subworkflows/local/quantification/main.nf:61:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      .join(OPENMS_MAPALIGNERPOSECLUSTERING.out.trafoxml.map{it[1]}.flatten().map{trafoxml ->
                                                             ^^
  ```

- Warning: `subworkflows/local/quantification/main.nf:63:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .join(quantificaiton_data.map{meta,mzml->
                                    ^^^^
  ```

- Warning: `subworkflows/local/quantification/main.nf:64:34`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  tuple(mzml.baseName, mzml)}).map{it[1..4]}
                                   ^^
  ```

- Warning: `subworkflows/local/quantification/main.nf:67:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      combined_data.map{it[0,2,3]} | OPENMS_MAPRTTRANSFORMER
                        ^^
  ```

- Warning: `subworkflows/local/quantification/main.nf:72:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      quantified_features=combined_data.map{it[0,1]}
                                            ^^
  ```

- Warning: `subworkflows/local/requantification/main.nf:14:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/requantification/main.nf:20:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  quantified_features.combine(data_split.map{it[1]}) |  PYOPENMS_RELOADMAPS
                                             ^^
  ```

- Warning: `subworkflows/local/requantification/main.nf:26:16`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  data_split.map{it[0,2]} | PYOPENMS_LIBBUILDER
                 ^^
  ```

- Warning: `subworkflows/local/requantification/main.nf:30:61`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  quantificaiton_data.combine(PYOPENMS_LIBBUILDER.out.tsv.map{it[1]}) | OPENMS_FEATUREFINDERMETABOIDENT
                                                              ^^
  ```

- Warning: `subworkflows/local/sirius/main.nf:19:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  ch_versions = Channel.empty()
                ^^^^^^^
  ```

- Warning: `subworkflows/local/sirius/main.nf:28:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  ms_channel = PYOPENMS_SPLITMS.out.ms.flatMap{id, values -> values.collect { [id, it]}}
                                                                                   ^^
  ```
