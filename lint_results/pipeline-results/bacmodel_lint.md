# Nextflow lint results

- Generated: 2026-07-23T00:29:52.302512821Z
- Nextflow version: 26.07.0-edge
- Summary: 57 warnings

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

- Warning: `modules/nf-core/gapseq/doall/main.nf:27:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/gapseq/findtransport/main.nf:24:9`: Variable was declared but not used

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

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:150:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gapseq_model = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:151:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gapseq_xml = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:152:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gapseq_tbl = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:158:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_memote_report = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:159:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_memote_json = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:165:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def final_xml = xml instanceof List ? xml.findAll { !it.name.contains('-draft') } : xml
                                                                       ^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:169:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, xml ->
                        ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:198:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_sample_ids = ch_genomes.map { meta, fasta -> meta.id }.collectFile(name: 'sample_ids.txt', newLine: true)
                                             ^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:201:63`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_macsyfinder_for_summary = ch_macsyfinder_results.map { meta, file -> file }.collect().ifEmpty([])
                                                                ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:202:64`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_traitar_majority_for_summary = ch_traitar_results.map { meta, file -> file }.collect().ifEmpty([])
                                                                 ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:203:67`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_traitar_single_for_summary = ch_traitar_single_votes.map { meta, file -> file }.collect().ifEmpty([])
                                                                    ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:204:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_carveme_for_summary = ch_carveme_model.map { meta, file -> file }.collect().ifEmpty([])
                                                      ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:210:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def final_xml = xml instanceof List ? xml.findAll { !it.name.contains('-draft') } : xml
                                                                   ^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:214:65`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_gapseq_for_summary = RENAME_GAPSEQ_XML.out.xml.map { meta, xml -> xml }.flatten().collect().ifEmpty([])
                                                                  ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:216:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gapseq_for_summary = Channel.empty()
                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:219:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_gapseq_tbl_for_summary = ch_gapseq_tbl.map { meta, files -> files }.flatten().collect().ifEmpty([])
                                                      ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:220:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_memote_for_summary = ch_memote_json.map { meta, json -> json }.collect().ifEmpty([])
                                                   ^^^^
  ```

- Warning: `subworkflows/local/gapseq_workflow/main.nf:35:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/gapseq_workflow/main.nf:66:60`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_find_input = ch_gapseq_input.map { meta, fasta, medium ->
                                                             ^^^^^^
  ```

- Warning: `subworkflows/local/gapseq_workflow/main.nf:72:69`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_findtransport_input = ch_gapseq_input.map { meta, fasta, medium ->
                                                                      ^^^^^^
  ```

- Warning: `subworkflows/local/gapseq_workflow/main.nf:93:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .join(ch_gapseq_input.map { meta, fasta, medium -> [ meta, medium ] }, by: 0)
                                                ^^^^^
  ```

- Warning: `subworkflows/local/gapseq_workflow/main.nf:131:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def pathways_tbl = files.find { it.name.contains('Pathways') }
                                              ^^
  ```

- Warning: `subworkflows/local/gapseq_workflow/main.nf:136:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def transport_tbl = files.find { it.name.contains('Transporter') }
                                               ^^
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

- Warning: `workflows/bacmodel.nf:39:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```
