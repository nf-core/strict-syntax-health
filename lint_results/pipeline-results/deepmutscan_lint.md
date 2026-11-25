# Nextflow lint results

- Generated: 2026-11-25T00:12:25.911337579Z
- Nextflow version: 26.11.0-edge
- Summary: 82 warnings

## :warning: Warnings

- Warning: `modules/local/dmsanalysis/error_correction_false_doubles/main.nf:26:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/dmsanalysis/error_correction_wildtype/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/dmsanalysis/error_signatures/main.nf:29:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/dmsanalysis/fdm_estimate/main.nf:27:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/dmsanalysis/fdm_evidence/main.nf:26:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/dmsanalysis/process_variant_counts/main.nf:26:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/dmsanalysis/reference_tables/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/fitness/counts_to_fitness/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/merge_align_count/main.nf:33:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/prepare_reference/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/raw_data_qc/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/structure/variant_effect_inspection_tool/main.nf:27:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/visualization/error_correction_report/main.nf:32:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/visualization/library_qc/main.nf:31:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/visualization/summary_report/main.nf:28:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/multiqc/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:28:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:42:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def inputs  = pairs.findAll { it[0].type == 'input'  }.sort { it[0].replicate }.collect { it[1] }
                                            ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:42:75`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def inputs  = pairs.findAll { it[0].type == 'input'  }.sort { it[0].replicate }.collect { it[1] }
                                                                            ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:42:103`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def inputs  = pairs.findAll { it[0].type == 'input'  }.sort { it[0].replicate }.collect { it[1] }
                                                                                                        ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:43:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def outputs = pairs.findAll { it[0].type == 'output' }.sort { it[0].replicate }.collect { it[1] }
                                            ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:43:75`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def outputs = pairs.findAll { it[0].type == 'output' }.sort { it[0].replicate }.collect { it[1] }
                                                                            ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:43:103`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def outputs = pairs.findAll { it[0].type == 'output' }.sort { it[0].replicate }.collect { it[1] }
                                                                                                        ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:46:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { smeta, ins, outs -> ins && outs }
                    ^^^^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:75:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_dimsum_dir    = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:76:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_mutscan_plots = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_deepmutscan_pipeline/main.nf:37:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:57:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_versions = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:58:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_multiqc_files = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:72:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.value(tuple([id: 'ref'], file(params.fasta, checkIfExists: true)))
          ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:83:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def reading_frame_ch        = Channel.value(params.reading_frame)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:84:65`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def custom_codon_library_ch = params.custom_codon_library ? Channel.value(file(params.custom_codon_library, checkIfExists: true)) : Channel.value([])
                                                                  ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:84:137`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def custom_codon_library_ch = params.custom_codon_library ? Channel.value(file(params.custom_codon_library, checkIfExists: true)) : Channel.value([])
                                                                                                                                          ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:85:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def mutagenesis_type_ch     = Channel.value(params.mutagenesis_type)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:86:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def sliding_window_size_ch  = Channel.value(asInt(params.sliding_window_size))
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:87:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def aimed_cov_ch            = Channel.value(asInt(params.aimed_cov))
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:88:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def base_qual_ch            = Channel.value(asInt(params.base_qual))
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:89:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def min_flank_ch            = Channel.value(asInt(params.min_flank))
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:92:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_samplesheet_csv      = Channel.value(file(params.input, checkIfExists: true))
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:175:9`: Variable was declared but not used

  ```nextflow
      def annotated_variantCounts_ch           = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, a) }
          ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:175:126`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def annotated_variantCounts_ch           = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, a) }
                                                                                                                               ^
  ```

- Warning: `workflows/deepmutscan.nf:175:129`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def annotated_variantCounts_ch           = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, a) }
                                                                                                                                  ^
  ```

- Warning: `workflows/deepmutscan.nf:175:132`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def annotated_variantCounts_ch           = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, a) }
                                                                                                                                     ^
  ```

- Warning: `workflows/deepmutscan.nf:176:123`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_filtered_by_library_ch = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, b) }
                                                                                                                            ^
  ```

- Warning: `workflows/deepmutscan.nf:176:129`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_filtered_by_library_ch = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, b) }
                                                                                                                                  ^
  ```

- Warning: `workflows/deepmutscan.nf:176:132`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_filtered_by_library_ch = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, b) }
                                                                                                                                     ^
  ```

- Warning: `workflows/deepmutscan.nf:177:123`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def library_completed_variantCounts_ch   = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, c) }
                                                                                                                            ^
  ```

- Warning: `workflows/deepmutscan.nf:177:126`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def library_completed_variantCounts_ch   = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, c) }
                                                                                                                               ^
  ```

- Warning: `workflows/deepmutscan.nf:177:132`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def library_completed_variantCounts_ch   = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, c) }
                                                                                                                                     ^
  ```

- Warning: `workflows/deepmutscan.nf:178:123`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_for_heatmaps_ch        = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, d) }
                                                                                                                            ^
  ```

- Warning: `workflows/deepmutscan.nf:178:126`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_for_heatmaps_ch        = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, d) }
                                                                                                                               ^
  ```

- Warning: `workflows/deepmutscan.nf:178:129`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_for_heatmaps_ch        = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, d) }
                                                                                                                                  ^
  ```

- Warning: `workflows/deepmutscan.nf:195:41`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_fd_in.map { meta, raw, filt, comp -> tuple(meta, raw, filt) },
                                          ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:263:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, raw, filt, comp, ev -> tuple(falseDoublesPool(meta, params.false_doubles_pooling), meta, filt, comp, ev) }
                       ^^^
  ```

- Warning: `workflows/deepmutscan.nf:270:121`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_filtered_by_library_ch = DMSANALYSIS_ERROR_CORRECTION_FALSE_DOUBLES.out.corrected.map { meta, filt, heat, comp -> tuple(meta, filt) }
                                                                                                                          ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:270:127`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_filtered_by_library_ch = DMSANALYSIS_ERROR_CORRECTION_FALSE_DOUBLES.out.corrected.map { meta, filt, heat, comp -> tuple(meta, filt) }
                                                                                                                                ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:271:115`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_for_heatmaps_ch        = DMSANALYSIS_ERROR_CORRECTION_FALSE_DOUBLES.out.corrected.map { meta, filt, heat, comp -> tuple(meta, heat) }
                                                                                                                    ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:271:127`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_for_heatmaps_ch        = DMSANALYSIS_ERROR_CORRECTION_FALSE_DOUBLES.out.corrected.map { meta, filt, heat, comp -> tuple(meta, heat) }
                                                                                                                                ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:272:115`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        library_completed_variantCounts_ch   = DMSANALYSIS_ERROR_CORRECTION_FALSE_DOUBLES.out.corrected.map { meta, filt, heat, comp -> tuple(meta, comp) }
                                                                                                                    ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:272:121`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        library_completed_variantCounts_ch   = DMSANALYSIS_ERROR_CORRECTION_FALSE_DOUBLES.out.corrected.map { meta, filt, heat, comp -> tuple(meta, comp) }
                                                                                                                          ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:277:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        def wt_ch     = filt_comp.filter { meta, f, c -> meta.type == 'wildtype' }.map { meta, f, c -> tuple(meta.sample, f) }
                                                 ^
  ```

- Warning: `workflows/deepmutscan.nf:277:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        def wt_ch     = filt_comp.filter { meta, f, c -> meta.type == 'wildtype' }.map { meta, f, c -> tuple(meta.sample, f) }
                                                    ^
  ```

- Warning: `workflows/deepmutscan.nf:277:97`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        def wt_ch     = filt_comp.filter { meta, f, c -> meta.type == 'wildtype' }.map { meta, f, c -> tuple(meta.sample, f) }
                                                                                                  ^
  ```

- Warning: `workflows/deepmutscan.nf:278:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        def tgt_ch    = filt_comp.filter { meta, f, c -> meta.type != 'wildtype' }.map { meta, f, c -> tuple(meta.sample, meta, f, c) }
                                                 ^
  ```

- Warning: `workflows/deepmutscan.nf:278:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        def tgt_ch    = filt_comp.filter { meta, f, c -> meta.type != 'wildtype' }.map { meta, f, c -> tuple(meta.sample, meta, f, c) }
                                                    ^
  ```

- Warning: `workflows/deepmutscan.nf:282:116`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_filtered_by_library_ch = DMSANALYSIS_ERROR_CORRECTION_WILDTYPE.out.corrected.map { meta, filt, heat, comp -> tuple(meta, filt) }
                                                                                                                     ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:282:122`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_filtered_by_library_ch = DMSANALYSIS_ERROR_CORRECTION_WILDTYPE.out.corrected.map { meta, filt, heat, comp -> tuple(meta, filt) }
                                                                                                                           ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:283:110`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_for_heatmaps_ch        = DMSANALYSIS_ERROR_CORRECTION_WILDTYPE.out.corrected.map { meta, filt, heat, comp -> tuple(meta, heat) }
                                                                                                               ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:283:122`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_for_heatmaps_ch        = DMSANALYSIS_ERROR_CORRECTION_WILDTYPE.out.corrected.map { meta, filt, heat, comp -> tuple(meta, heat) }
                                                                                                                           ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:284:110`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        library_completed_variantCounts_ch   = DMSANALYSIS_ERROR_CORRECTION_WILDTYPE.out.corrected.map { meta, filt, heat, comp -> tuple(meta, comp) }
                                                                                                               ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:284:116`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        library_completed_variantCounts_ch   = DMSANALYSIS_ERROR_CORRECTION_WILDTYPE.out.corrected.map { meta, filt, heat, comp -> tuple(meta, comp) }
                                                                                                                     ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:290:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_report_assets = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:302:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_ec.map { rows -> groovy.json.JsonOutput.toJson(rows.collect { [id: it[0].id, type: it[0].type, replicate: it[0].replicate] }).bytes.encodeBase64().toString() },
                                                                                ^^
  ```

- Warning: `workflows/deepmutscan.nf:302:95`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_ec.map { rows -> groovy.json.JsonOutput.toJson(rows.collect { [id: it[0].id, type: it[0].type, replicate: it[0].replicate] }).bytes.encodeBase64().toString() },
                                                                                                ^^
  ```

- Warning: `workflows/deepmutscan.nf:302:118`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_ec.map { rows -> groovy.json.JsonOutput.toJson(rows.collect { [id: it[0].id, type: it[0].type, replicate: it[0].replicate] }).bytes.encodeBase64().toString() },
                                                                                                                       ^^
  ```

- Warning: `workflows/deepmutscan.nf:303:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_ec.map { rows -> rows.collect { it[1] } },
                                             ^^
  ```

- Warning: `workflows/deepmutscan.nf:389:68`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
            .mix(CALCULATE_FITNESS.out.dimsum_dir.flatten().filter { it.name == 'report.html' }.map { f -> [['report', 'dimsum', 'DiMSum'], f] })
                                                                     ^^
  ```

- Warning: `workflows/deepmutscan.nf:397:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              def ch_structure = Channel
                                 ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:495:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def manifest = rows.collect { [kind: it[0][0], group: it[0][1], name: it[0][2]] }
                                                   ^^
  ```

- Warning: `workflows/deepmutscan.nf:495:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def manifest = rows.collect { [kind: it[0][0], group: it[0][1], name: it[0][2]] }
                                                                    ^^
  ```

- Warning: `workflows/deepmutscan.nf:495:83`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def manifest = rows.collect { [kind: it[0][0], group: it[0][1], name: it[0][2]] }
                                                                                    ^^
  ```

- Warning: `workflows/deepmutscan.nf:498:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  rows.collect { it[1] },
                                 ^^
  ```
