# Nextflow lint results

- Generated: 2026-06-26T00:41:33.153771468Z
- Nextflow version: 26.05.0-edge
- Summary: 54 warnings

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

- Warning: `modules/local/rename_gapseq_xml/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
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

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:31:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:32:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_annotated_proteins = Channel.empty()
                              ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:33:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_annotated_gff = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:34:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_macsyfinder_results = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:35:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_traitar_results = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:36:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_traitar_single_votes = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:37:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_carveme_model = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:38:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gapseq_model = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:39:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gapseq_tbl = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:52:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_baktadb = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:60:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_baktadb = Channel.fromPath(params.baktadb, checkIfExists: true)
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:86:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_macsyfinder_results = Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:92:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_pfamdb = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:100:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_pfamdb = Channel.fromPath(params.pfamdb, checkIfExists: true)
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:113:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_traitar_results = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:114:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_traitar_single_votes = Channel.empty()
                                    ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:128:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_carveme_model = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:148:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gapseq_model = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:149:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gapseq_xml = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:150:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gapseq_tbl = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:156:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_memote_report = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:157:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_memote_json = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:163:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def final_xml = xml instanceof List ? xml.findAll { !it.name.contains('-draft') } : xml
                                                                       ^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:167:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, xml ->
                        ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:196:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_sample_ids = ch_genomes.map { meta, fasta -> meta.id }.collectFile(name: 'sample_ids.txt', newLine: true)
                                             ^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:199:63`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_macsyfinder_for_summary = ch_macsyfinder_results.map { meta, file -> file }.collect().ifEmpty([])
                                                                ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:200:64`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_traitar_majority_for_summary = ch_traitar_results.map { meta, file -> file }.collect().ifEmpty([])
                                                                 ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:201:67`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_traitar_single_for_summary = ch_traitar_single_votes.map { meta, file -> file }.collect().ifEmpty([])
                                                                    ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:202:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_carveme_for_summary = ch_carveme_model.map { meta, file -> file }.collect().ifEmpty([])
                                                      ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:208:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def final_xml = xml instanceof List ? xml.findAll { !it.name.contains('-draft') } : xml
                                                                   ^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:212:65`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_gapseq_for_summary = RENAME_GAPSEQ_XML.out.xml.map { meta, xml -> xml }.flatten().collect().ifEmpty([])
                                                                  ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:214:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gapseq_for_summary = Channel.empty()
                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:217:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_gapseq_tbl_for_summary = ch_gapseq_tbl.map { meta, files -> files }.flatten().collect().ifEmpty([])
                                                      ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:218:50`: Parameter was not used -- prefix with `_` to suppress warning

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

- Warning: `workflows/bacmodel.nf:70:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions       = ch_collated_versions                 // channel: [ path(versions.yml) ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```
