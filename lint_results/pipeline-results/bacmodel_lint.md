# Nextflow lint results

- Generated: 2026-08-20T00:09:58.806508678Z
- Nextflow version: 26.07.0-edge
- Summary: 2 errors, 54 warnings

## :x: Errors

- Error: `main.nf:40:5`: Incorrect number of call arguments, expected 1 but received 2

  ```nextflow
      BACMODEL (
      ^
  ```

- Error: `workflows/bacmodel.nf:80:26`: `outdir` is not defined

  ```nextflow
              storeDir: "${outdir}/pipeline_info",
                           ^^^^^^
  ```

## :warning: Warnings

- Warning: `modules/local/bacmodel_summary/main.nf:33:5`: Variable was declared but not used

  ```nextflow
      macsyfinder_files = macsyfinder_results ? macsyfinder_results.collect { "'$it'" }.join(' ') : ''
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:33:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      macsyfinder_files = macsyfinder_results ? macsyfinder_results.collect { "'$it'" }.join(' ') : ''
                                                                                ^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:34:5`: Variable was declared but not used

  ```nextflow
      traitar_majority_files = traitar_majority_results ? traitar_majority_results.collect { "'$it'" }.join(' ') : ''
      ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:34:94`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      traitar_majority_files = traitar_majority_results ? traitar_majority_results.collect { "'$it'" }.join(' ') : ''
                                                                                               ^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:35:5`: Variable was declared but not used

  ```nextflow
      traitar_single_files = traitar_single_results ? traitar_single_results.collect { "'$it'" }.join(' ') : ''
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:35:88`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      traitar_single_files = traitar_single_results ? traitar_single_results.collect { "'$it'" }.join(' ') : ''
                                                                                         ^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:36:5`: Variable was declared but not used

  ```nextflow
      carveme_files = carveme_models ? carveme_models.collect { "'$it'" }.join(' ') : ''
      ^^^^^^^^^^^^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:36:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      carveme_files = carveme_models ? carveme_models.collect { "'$it'" }.join(' ') : ''
                                                                  ^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:37:5`: Variable was declared but not used

  ```nextflow
      gapseq_files = gapseq_models ? gapseq_models.collect { "'$it'" }.join(' ') : ''
      ^^^^^^^^^^^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:37:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      gapseq_files = gapseq_models ? gapseq_models.collect { "'$it'" }.join(' ') : ''
                                                               ^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:38:5`: Variable was declared but not used

  ```nextflow
      gapseq_tbl_files = gapseq_tbls ? gapseq_tbls.collect { "'$it'" }.join(' ') : ''
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:38:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      gapseq_tbl_files = gapseq_tbls ? gapseq_tbls.collect { "'$it'" }.join(' ') : ''
                                                               ^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:39:5`: Variable was declared but not used

  ```nextflow
      memote_files = memote_jsons ? memote_jsons.collect { "'$it'" }.join(' ') : ''
      ^^^^^^^^^^^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:39:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      memote_files = memote_jsons ? memote_jsons.collect { "'$it'" }.join(' ') : ''
                                                             ^^
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

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:57:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_baktadb = Channel.fromPath(baktadb_cached, checkIfExists: true)
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:81:37`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_macsyfinder_models = Channel.fromPath(macsyfinder_models_cached, checkIfExists: true)
                                      ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:94:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_macsyfinder_results = Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:105:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_pfamdb = Channel.fromPath(pfamdb_cached, checkIfExists: true)
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:119:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_traitar_results = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:120:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_traitar_single_votes = Channel.empty()
                                    ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:138:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_carveme_model = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:160:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gapseq_model = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:161:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gapseq_xml = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:162:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gapseq_tbl = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:168:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_memote_report = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:169:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_memote_json = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:175:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def final_xml = xml instanceof List ? xml.findAll { !it.name.contains('-draft') } : xml
                                                                       ^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:179:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, xml ->
                        ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:208:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_sample_ids = ch_genomes.map { meta, fasta -> meta.id }.collectFile(name: 'sample_ids.txt', newLine: true)
                                             ^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:211:63`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_macsyfinder_for_summary = ch_macsyfinder_results.map { meta, file -> file }.collect().ifEmpty([])
                                                                ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:212:64`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_traitar_majority_for_summary = ch_traitar_results.map { meta, file -> file }.collect().ifEmpty([])
                                                                 ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:213:67`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_traitar_single_for_summary = ch_traitar_single_votes.map { meta, file -> file }.collect().ifEmpty([])
                                                                    ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:214:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_carveme_for_summary = ch_carveme_model.map { meta, file -> file }.collect().ifEmpty([])
                                                      ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:220:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def final_xml = xml instanceof List ? xml.findAll { !it.name.contains('-draft') } : xml
                                                                   ^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:224:65`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_gapseq_for_summary = RENAME_GAPSEQ_XML.out.xml.map { meta, xml -> xml }.flatten().collect().ifEmpty([])
                                                                  ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:226:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gapseq_for_summary = Channel.empty().collect().ifEmpty([])
                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:229:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_gapseq_tbl_for_summary = ch_gapseq_tbl.map { meta, files -> files }.flatten().collect().ifEmpty([])
                                                      ^^^^
  ```

- Warning: `subworkflows/local/bacmodel_annotation/main.nf:230:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_memote_for_summary = ch_memote_json.map { meta, json -> json }.collect().ifEmpty([])
                                                   ^^^^
  ```

- Warning: `subworkflows/local/gapseq_workflow/main.nf:37:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/gapseq_workflow/main.nf:70:60`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_find_input = ch_gapseq_input.map { meta, fasta, medium ->
                                                             ^^^^^^
  ```

- Warning: `subworkflows/local/gapseq_workflow/main.nf:76:69`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_findtransport_input = ch_gapseq_input.map { meta, fasta, medium ->
                                                                      ^^^^^^
  ```

- Warning: `subworkflows/local/gapseq_workflow/main.nf:97:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .join(ch_gapseq_input.map { meta, fasta, medium -> [ meta, medium ] }, by: 0)
                                                ^^^^^
  ```

- Warning: `subworkflows/local/gapseq_workflow/main.nf:135:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def pathways_tbl = files.find { it.name.contains('Pathways') }
                                              ^^
  ```

- Warning: `subworkflows/local/gapseq_workflow/main.nf:140:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def transport_tbl = files.find { it.name.contains('Transporter') }
                                               ^^
  ```
