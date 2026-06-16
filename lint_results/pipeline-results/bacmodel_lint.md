# Nextflow lint results

- Generated: 2026-06-16T20:17:28.513983906Z
- Nextflow version: 26.04.3
- Summary: 56 warnings

## :warning: Warnings

- Warning: `modules/local/bacmodel_summary/main.nf:34:83`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def macsyfinder_files = macsyfinder_results ? macsyfinder_results.collect { "'$it'" }.join(' ') : ''
                                                                                    ^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:35:98`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def traitar_majority_files = traitar_majority_results ? traitar_majority_results.collect { "'$it'" }.join(' ') : ''
                                                                                                   ^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:36:92`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def traitar_single_files = traitar_single_results ? traitar_single_results.collect { "'$it'" }.join(' ') : ''
                                                                                             ^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:37:69`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def carveme_files = carveme_models ? carveme_models.collect { "'$it'" }.join(' ') : ''
                                                                      ^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:38:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def gapseq_files = gapseq_models ? gapseq_models.collect { "'$it'" }.join(' ') : ''
                                                                   ^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:39:9`: Variable was declared but not used

  ```nextflow
      def gapseq_tbl_files = gapseq_tbls ? gapseq_tbls.collect { "'$it'" }.join(' ') : ''
          ^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:39:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def gapseq_tbl_files = gapseq_tbls ? gapseq_tbls.collect { "'$it'" }.join(' ') : ''
                                                                   ^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def memote_files = memote_jsons ? memote_jsons.collect { "'$it'" }.join(' ') : ''
          ^^^^^^^^^^^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:40:64`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def memote_files = memote_jsons ? memote_jsons.collect { "'$it'" }.join(' ') : ''
                                                                 ^^
  ```

- Warning: `modules/nf-core/gapseq/doall/main.nf:26:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_analysis/main.nf:18:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:30:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:31:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_annotated_proteins = Channel.empty()
                              ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:32:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_annotated_gff = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:33:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_macsyfinder_results = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:34:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_traitar_results = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:35:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_traitar_single_votes = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:36:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_carveme_model = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:37:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gapseq_model = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:38:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gapseq_tbl = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:51:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_baktadb = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:59:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_baktadb = Channel.fromPath(params.baktadb, checkIfExists: true)
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:85:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_macsyfinder_results = Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:91:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_pfamdb = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:99:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_pfamdb = Channel.fromPath(params.pfamdb, checkIfExists: true)
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:112:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_traitar_results = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:113:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_traitar_single_votes = Channel.empty()
                                    ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:119:9`: Variable was declared but not used

  ```nextflow
          ch_carveme_mediadb = params.carveme_mediadb
          ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:120:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ? Channel.fromPath(params.carveme_mediadb, checkIfExists: true)
                ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:121:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              : Channel.empty()
                ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:132:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_carveme_model = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:152:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gapseq_model = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:153:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gapseq_xml = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:154:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gapseq_tbl = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:160:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_memote_report = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:161:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_memote_json = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:167:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def final_xml = xml instanceof List ? xml.findAll { !it.name.contains('-draft') } : xml
                                                                       ^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:171:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, xml ->
                        ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:200:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_sample_ids = ch_genomes.map { meta, fasta -> meta.id }.collect()
                                             ^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:203:63`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_macsyfinder_for_summary = ch_macsyfinder_results.map { meta, file -> file }.collect().ifEmpty([])
                                                                ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:204:64`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_traitar_majority_for_summary = ch_traitar_results.map { meta, file -> file }.collect().ifEmpty([])
                                                                 ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:205:67`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_traitar_single_for_summary = ch_traitar_single_votes.map { meta, file -> file }.collect().ifEmpty([])
                                                                    ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:206:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_carveme_for_summary = ch_carveme_model.map { meta, file -> file }.collect().ifEmpty([])
                                                      ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:208:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_gapseq_for_summary = ch_gapseq_xml.map { meta, xml ->
                                                  ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:210:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def final_xml = xml instanceof List ? xml.findAll { !it.name.contains('-draft') } : xml
                                                               ^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:218:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_gapseq_tbl_for_summary = ch_gapseq_tbl.map { meta, files -> files }.flatten().collect().ifEmpty([])
                                                      ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:219:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_memote_for_summary = ch_memote_json.map { meta, json -> json }.collect().ifEmpty([])
                                                   ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_bacmodel_pipeline/main.nf:30:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_bacmodel_pipeline/main.nf:33:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_bacmodel_pipeline/main.nf:125:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      hook_url        //  string: hook URL for notifications
      ^^^^^^^^
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

- Warning: `workflows/bacmodel.nf:39:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```

- Warning: `workflows/bacmodel.nf:66:17`: Variable was declared but not used

  ```nextflow
          ).set { ch_collated_versions }
                  ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/bacmodel.nf:70:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions       = ch_versions                 // channel: [ path(versions.yml) ]
      ^^^^^^^^^^^^^^^^^^^^
  ```
