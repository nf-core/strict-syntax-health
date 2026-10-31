# Nextflow lint results

- Generated: 2026-10-31T00:11:55.475580958Z
- Nextflow version: 26.10.4
- Summary: 77 warnings

## :warning: Warnings

- Warning: `modules/local/bacmodel_summary/main.nf:32:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:36:5`: Variable was declared but not used

  ```nextflow
      macsyfinder_files = macsyfinder_results ? macsyfinder_results.collect { "'$it'" }.join(' ') : ''
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:36:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      macsyfinder_files = macsyfinder_results ? macsyfinder_results.collect { "'$it'" }.join(' ') : ''
                                                                                ^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:37:5`: Variable was declared but not used

  ```nextflow
      macsyfinder_ids_str = macsyfinder_ids ? macsyfinder_ids.collect { "'$it'" }.join(' ') : ''
      ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:37:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      macsyfinder_ids_str = macsyfinder_ids ? macsyfinder_ids.collect { "'$it'" }.join(' ') : ''
                                                                          ^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:38:5`: Variable was declared but not used

  ```nextflow
      traitar_majority_files = traitar_majority_results ? traitar_majority_results.collect { "'$it'" }.join(' ') : ''
      ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:38:94`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      traitar_majority_files = traitar_majority_results ? traitar_majority_results.collect { "'$it'" }.join(' ') : ''
                                                                                               ^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:39:5`: Variable was declared but not used

  ```nextflow
      traitar_single_files = traitar_single_results ? traitar_single_results.collect { "'$it'" }.join(' ') : ''
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:39:88`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      traitar_single_files = traitar_single_results ? traitar_single_results.collect { "'$it'" }.join(' ') : ''
                                                                                         ^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:40:5`: Variable was declared but not used

  ```nextflow
      carveme_files = carveme_models ? carveme_models.collect { "'$it'" }.join(' ') : ''
      ^^^^^^^^^^^^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:40:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      carveme_files = carveme_models ? carveme_models.collect { "'$it'" }.join(' ') : ''
                                                                  ^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:41:5`: Variable was declared but not used

  ```nextflow
      carveme_ids_str = carveme_ids ? carveme_ids.collect { "'$it'" }.join(' ') : ''
      ^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:41:61`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      carveme_ids_str = carveme_ids ? carveme_ids.collect { "'$it'" }.join(' ') : ''
                                                              ^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:42:5`: Variable was declared but not used

  ```nextflow
      gapseq_files = gapseq_models ? gapseq_models.collect { "'$it'" }.join(' ') : ''
      ^^^^^^^^^^^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:42:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      gapseq_files = gapseq_models ? gapseq_models.collect { "'$it'" }.join(' ') : ''
                                                               ^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:43:5`: Variable was declared but not used

  ```nextflow
      gapseq_ids_str = gapseq_ids ? gapseq_ids.collect { "'$it'" }.join(' ') : ''
      ^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:43:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      gapseq_ids_str = gapseq_ids ? gapseq_ids.collect { "'$it'" }.join(' ') : ''
                                                           ^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:44:5`: Variable was declared but not used

  ```nextflow
      gapseq_tbl_files = gapseq_tbls ? gapseq_tbls.collect { "'$it'" }.join(' ') : ''
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:44:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      gapseq_tbl_files = gapseq_tbls ? gapseq_tbls.collect { "'$it'" }.join(' ') : ''
                                                               ^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:45:5`: Variable was declared but not used

  ```nextflow
      memote_files = memote_jsons ? memote_jsons.collect { "'$it'" }.join(' ') : ''
      ^^^^^^^^^^^^
  ```

- Warning: `modules/local/bacmodel_summary/main.nf:45:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      memote_files = memote_jsons ? memote_jsons.collect { "'$it'" }.join(' ') : ''
                                                             ^^
  ```

- Warning: `modules/nf-core/bakta/bakta/main.nf:31:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bakta/baktadbdownload/main.nf:13:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/carveme/carve/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gapseq/doall/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gapseq/doall/main.nf:27:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/gapseq/draft/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gapseq/fill/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gapseq/find/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gapseq/findtransport/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gapseq/findtransport/main.nf:24:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/gapseq/medium/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gapseq/requestdb/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/macsyfinder/download/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/macsyfinder/search/main.nf:25:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/memote/report/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/memote/run/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/prokka/main.nf:30:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/traitar/pfamget/main.nf:14:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/traitar/run/main.nf:24:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `subworkflows/local/annotation/main.nf:22:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_proteins = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/annotation/main.nf:23:14`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gff = Channel.empty()
               ^^^^^^^
  ```

- Warning: `subworkflows/local/annotation/main.nf:32:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_bakta_db = Channel.fromPath(bakta_db_cached, checkIfExists: true)
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/gapseq_workflow/main.nf:53:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_seqdb = Channel.fromPath(gapseq_db, checkIfExists: true).first()
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/gapseq_workflow/main.nf:77:60`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_find_input = ch_gapseq_input.map { meta, fasta, medium ->
                                                             ^^^^^^
  ```

- Warning: `subworkflows/local/gapseq_workflow/main.nf:83:69`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_findtransport_input = ch_gapseq_input.map { meta, fasta, medium ->
                                                                      ^^^^^^
  ```

- Warning: `subworkflows/local/gapseq_workflow/main.nf:104:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .join(ch_gapseq_input.map { meta, fasta, medium -> [ meta, medium ] }, by: 0)
                                                ^^^^^
  ```

- Warning: `subworkflows/local/gapseq_workflow/main.nf:142:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def pathways_tbl = files.find { it.name.contains('Pathways') }
                                              ^^
  ```

- Warning: `subworkflows/local/gapseq_workflow/main.nf:147:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def transport_tbl = files.find { it.name.contains('Transporter') }
                                               ^^
  ```

- Warning: `subworkflows/local/macsyfinder/main.nf:28:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_macsyfinder_models = Channel.fromPath(macsyfinder_models_cached, checkIfExists: true)
                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/traitar_workflow/main.nf:28:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_pfam_db = Channel.fromPath(pfam_db_cached, checkIfExists: true)
                       ^^^^^^^
  ```

- Warning: `workflows/bacmodel.nf:46:5`: Variable was declared but not used

  ```nextflow
      ch_gff = ANNOTATION.out.gff
      ^^^^^^
  ```

- Warning: `workflows/bacmodel.nf:57:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_macsyfinder_results = Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `workflows/bacmodel.nf:68:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_traitar_results = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `workflows/bacmodel.nf:69:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_traitar_single_votes = Channel.empty()
                                    ^^^^^^^
  ```

- Warning: `workflows/bacmodel.nf:89:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_carveme_model = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `workflows/bacmodel.nf:120:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gapseq_model = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `workflows/bacmodel.nf:121:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gapseq_xml = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `workflows/bacmodel.nf:122:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gapseq_tbl = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `workflows/bacmodel.nf:128:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_memote_report = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `workflows/bacmodel.nf:129:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_memote_json = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `workflows/bacmodel.nf:135:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def final_xml = xml instanceof List ? xml.findAll { !it.name.contains('-draft') } : xml
                                                                       ^^
  ```

- Warning: `workflows/bacmodel.nf:139:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, xml ->
                        ^^^^
  ```

- Warning: `workflows/bacmodel.nf:166:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_sample_ids = ch_genomes.map { meta, fasta -> meta.id }.collectFile(name: 'sample_ids.txt', newLine: true)
                                             ^^^^^
  ```

- Warning: `workflows/bacmodel.nf:173:63`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_macsyfinder_for_summary = ch_macsyfinder_results.map { meta, file -> file }.collect().ifEmpty([])
                                                                ^^^^
  ```

- Warning: `workflows/bacmodel.nf:174:73`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_macsyfinder_ids_for_summary = ch_macsyfinder_results.map { meta, file -> meta.id }.collect().ifEmpty([])
                                                                          ^^^^
  ```

- Warning: `workflows/bacmodel.nf:175:64`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_traitar_majority_for_summary = ch_traitar_results.map { meta, file -> file }.collect().ifEmpty([])
                                                                 ^^^^
  ```

- Warning: `workflows/bacmodel.nf:176:67`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_traitar_single_for_summary = ch_traitar_single_votes.map { meta, file -> file }.collect().ifEmpty([])
                                                                    ^^^^
  ```

- Warning: `workflows/bacmodel.nf:177:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_carveme_for_summary = ch_carveme_model.map { meta, file -> file }.collect().ifEmpty([])
                                                      ^^^^
  ```

- Warning: `workflows/bacmodel.nf:178:63`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_carveme_ids_for_summary = ch_carveme_model.map { meta, file -> meta.id }.collect().ifEmpty([])
                                                                ^^^^
  ```

- Warning: `workflows/bacmodel.nf:186:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def final_files = files.findAll { !it.name.contains('-draft') }
                                                 ^^
  ```

- Warning: `workflows/bacmodel.nf:192:55`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_gapseq_for_summary = ch_gapseq_pairs.map { id, file -> file }.collect().ifEmpty([])
                                                        ^^
  ```

- Warning: `workflows/bacmodel.nf:193:63`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_gapseq_ids_for_summary = ch_gapseq_pairs.map { id, file -> id }.collect().ifEmpty([])
                                                                ^^^^
  ```

- Warning: `workflows/bacmodel.nf:195:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gapseq_for_summary = Channel.empty().collect().ifEmpty([])
                                  ^^^^^^^
  ```

- Warning: `workflows/bacmodel.nf:196:37`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gapseq_ids_for_summary = Channel.empty().collect().ifEmpty([])
                                      ^^^^^^^
  ```

- Warning: `workflows/bacmodel.nf:199:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_gapseq_tbl_for_summary = ch_gapseq_tbl.map { meta, files -> files }.flatten().collect().ifEmpty([])
                                                      ^^^^
  ```

- Warning: `workflows/bacmodel.nf:200:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_memote_for_summary = ch_memote_json.map { meta, json -> json }.collect().ifEmpty([])
                                                   ^^^^
  ```
