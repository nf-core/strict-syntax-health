# Nextflow lint results

- Generated: 2026-11-13T00:14:13.308408186Z
- Nextflow version: 26.10.5
- Summary: 89 warnings

## :warning: Warnings

- Warning: `modules/local/bamprocessing/merge_align/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/dmsanalysis/aa_seq/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/dmsanalysis/error_correction_false_doubles/main.nf:27:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/dmsanalysis/error_correction_wildtype/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/dmsanalysis/possible_mutations/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/dmsanalysis/process_variant_counts/main.nf:26:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/fastq_check/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/fitness/counts_to_fitness/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/structure/variant_effect_inspection_tool/main.nf:27:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/variantcounting/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/visualization/counts_heatmap/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/visualization/counts_per_cov/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/visualization/error_correction_report/main.nf:28:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/visualization/global_pos_biases_counts/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/visualization/global_pos_biases_cov/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/visualization/logdiff/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/visualization/seqdepth/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/visualization/summary_report/main.nf:28:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bwa/index/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/fastqc/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/multiqc/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:33:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:47:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def inputs  = pairs.findAll { it[0].type == 'input'  }.sort { it[0].replicate }.collect { it[1] }
                                            ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:47:75`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def inputs  = pairs.findAll { it[0].type == 'input'  }.sort { it[0].replicate }.collect { it[1] }
                                                                            ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:47:103`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def inputs  = pairs.findAll { it[0].type == 'input'  }.sort { it[0].replicate }.collect { it[1] }
                                                                                                        ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:48:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def outputs = pairs.findAll { it[0].type == 'output' }.sort { it[0].replicate }.collect { it[1] }
                                            ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:48:75`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def outputs = pairs.findAll { it[0].type == 'output' }.sort { it[0].replicate }.collect { it[1] }
                                                                            ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:48:103`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def outputs = pairs.findAll { it[0].type == 'output' }.sort { it[0].replicate }.collect { it[1] }
                                                                                                        ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:51:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { smeta, ins, outs -> ins && outs }
                    ^^^^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:82:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { key, smp, counts, wt -> tuple(smp, counts, wt) }
                 ^^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:85:61`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def ch_run_counts_d = ch_counts_wt_d.map { smp, counts, wt -> tuple(smp, counts) }
                                                              ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:86:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def ch_run_wt_d     = ch_counts_wt_d.map { smp, counts, wt -> wt }
                                                 ^^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:86:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def ch_run_wt_d     = ch_counts_wt_d.map { smp, counts, wt -> wt }
                                                      ^^^^^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:110:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_dimsum_dir    = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:111:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_mutscan_plots = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_deepmutscan_pipeline/main.nf:37:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:55:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_versions = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:56:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_multiqc_files = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:62:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_fasta = Channel.value(tuple([id: 'ref'], file(params.fasta, checkIfExists: true)))
                     ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:71:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def reading_frame_ch        = Channel.value(params.reading_frame)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:72:65`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def custom_codon_library_ch = params.custom_codon_library ? Channel.value(file(params.custom_codon_library, checkIfExists: true)) : Channel.value([])
                                                                  ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:72:137`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def custom_codon_library_ch = params.custom_codon_library ? Channel.value(file(params.custom_codon_library, checkIfExists: true)) : Channel.value([])
                                                                                                                                          ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:73:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def mutagenesis_type_ch     = Channel.value(params.mutagenesis_type)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:74:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def sliding_window_size_ch  = Channel.value(asInt(params.sliding_window_size))
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:75:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def aimed_cov_ch            = Channel.value(asInt(params.aimed_cov))
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:76:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def base_qual_ch            = Channel.value(asInt(params.base_qual))
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:77:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def min_flank_ch            = Channel.value(asInt(params.min_flank))
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:80:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_samplesheet_csv      = Channel.value(file(params.input, checkIfExists: true))
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:177:9`: Variable was declared but not used

  ```nextflow
      def annotated_variantCounts_ch           = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, a) }
          ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:177:126`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def annotated_variantCounts_ch           = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, a) }
                                                                                                                               ^
  ```

- Warning: `workflows/deepmutscan.nf:177:129`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def annotated_variantCounts_ch           = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, a) }
                                                                                                                                  ^
  ```

- Warning: `workflows/deepmutscan.nf:177:132`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def annotated_variantCounts_ch           = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, a) }
                                                                                                                                     ^
  ```

- Warning: `workflows/deepmutscan.nf:178:123`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_filtered_by_library_ch = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, b) }
                                                                                                                            ^
  ```

- Warning: `workflows/deepmutscan.nf:178:129`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_filtered_by_library_ch = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, b) }
                                                                                                                                  ^
  ```

- Warning: `workflows/deepmutscan.nf:178:132`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_filtered_by_library_ch = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, b) }
                                                                                                                                     ^
  ```

- Warning: `workflows/deepmutscan.nf:179:123`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def library_completed_variantCounts_ch   = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, c) }
                                                                                                                            ^
  ```

- Warning: `workflows/deepmutscan.nf:179:126`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def library_completed_variantCounts_ch   = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, c) }
                                                                                                                               ^
  ```

- Warning: `workflows/deepmutscan.nf:179:132`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def library_completed_variantCounts_ch   = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, c) }
                                                                                                                                     ^
  ```

- Warning: `workflows/deepmutscan.nf:180:123`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_for_heatmaps_ch        = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, d) }
                                                                                                                            ^
  ```

- Warning: `workflows/deepmutscan.nf:180:126`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_for_heatmaps_ch        = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, d) }
                                                                                                                               ^
  ```

- Warning: `workflows/deepmutscan.nf:180:129`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_for_heatmaps_ch        = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, d) }
                                                                                                                                  ^
  ```

- Warning: `workflows/deepmutscan.nf:197:121`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_filtered_by_library_ch = DMSANALYSIS_ERROR_CORRECTION_FALSE_DOUBLES.out.corrected.map { meta, filt, heat, comp -> tuple(meta, filt) }
                                                                                                                          ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:197:127`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_filtered_by_library_ch = DMSANALYSIS_ERROR_CORRECTION_FALSE_DOUBLES.out.corrected.map { meta, filt, heat, comp -> tuple(meta, filt) }
                                                                                                                                ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:198:115`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_for_heatmaps_ch        = DMSANALYSIS_ERROR_CORRECTION_FALSE_DOUBLES.out.corrected.map { meta, filt, heat, comp -> tuple(meta, heat) }
                                                                                                                    ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:198:127`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_for_heatmaps_ch        = DMSANALYSIS_ERROR_CORRECTION_FALSE_DOUBLES.out.corrected.map { meta, filt, heat, comp -> tuple(meta, heat) }
                                                                                                                                ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:199:115`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        library_completed_variantCounts_ch   = DMSANALYSIS_ERROR_CORRECTION_FALSE_DOUBLES.out.corrected.map { meta, filt, heat, comp -> tuple(meta, comp) }
                                                                                                                    ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:199:121`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        library_completed_variantCounts_ch   = DMSANALYSIS_ERROR_CORRECTION_FALSE_DOUBLES.out.corrected.map { meta, filt, heat, comp -> tuple(meta, comp) }
                                                                                                                          ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:204:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        def wt_ch     = filt_comp.filter { meta, f, c -> meta.type == 'wildtype' }.map { meta, f, c -> tuple(meta.sample, f) }
                                                 ^
  ```

- Warning: `workflows/deepmutscan.nf:204:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        def wt_ch     = filt_comp.filter { meta, f, c -> meta.type == 'wildtype' }.map { meta, f, c -> tuple(meta.sample, f) }
                                                    ^
  ```

- Warning: `workflows/deepmutscan.nf:204:97`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        def wt_ch     = filt_comp.filter { meta, f, c -> meta.type == 'wildtype' }.map { meta, f, c -> tuple(meta.sample, f) }
                                                                                                  ^
  ```

- Warning: `workflows/deepmutscan.nf:205:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        def tgt_ch    = filt_comp.filter { meta, f, c -> meta.type != 'wildtype' }.map { meta, f, c -> tuple(meta.sample, meta, f, c) }
                                                 ^
  ```

- Warning: `workflows/deepmutscan.nf:205:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        def tgt_ch    = filt_comp.filter { meta, f, c -> meta.type != 'wildtype' }.map { meta, f, c -> tuple(meta.sample, meta, f, c) }
                                                    ^
  ```

- Warning: `workflows/deepmutscan.nf:209:116`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_filtered_by_library_ch = DMSANALYSIS_ERROR_CORRECTION_WILDTYPE.out.corrected.map { meta, filt, heat, comp -> tuple(meta, filt) }
                                                                                                                     ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:209:122`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_filtered_by_library_ch = DMSANALYSIS_ERROR_CORRECTION_WILDTYPE.out.corrected.map { meta, filt, heat, comp -> tuple(meta, filt) }
                                                                                                                           ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:210:110`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_for_heatmaps_ch        = DMSANALYSIS_ERROR_CORRECTION_WILDTYPE.out.corrected.map { meta, filt, heat, comp -> tuple(meta, heat) }
                                                                                                               ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:210:122`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_for_heatmaps_ch        = DMSANALYSIS_ERROR_CORRECTION_WILDTYPE.out.corrected.map { meta, filt, heat, comp -> tuple(meta, heat) }
                                                                                                                           ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:211:110`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        library_completed_variantCounts_ch   = DMSANALYSIS_ERROR_CORRECTION_WILDTYPE.out.corrected.map { meta, filt, heat, comp -> tuple(meta, comp) }
                                                                                                               ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:211:116`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        library_completed_variantCounts_ch   = DMSANALYSIS_ERROR_CORRECTION_WILDTYPE.out.corrected.map { meta, filt, heat, comp -> tuple(meta, comp) }
                                                                                                                     ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:217:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_report_assets = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:229:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_ec.map { rows -> groovy.json.JsonOutput.toJson(rows.collect { [id: it[0].id, type: it[0].type, replicate: it[0].replicate] }).bytes.encodeBase64().toString() },
                                                                                ^^
  ```

- Warning: `workflows/deepmutscan.nf:229:95`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_ec.map { rows -> groovy.json.JsonOutput.toJson(rows.collect { [id: it[0].id, type: it[0].type, replicate: it[0].replicate] }).bytes.encodeBase64().toString() },
                                                                                                ^^
  ```

- Warning: `workflows/deepmutscan.nf:229:118`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_ec.map { rows -> groovy.json.JsonOutput.toJson(rows.collect { [id: it[0].id, type: it[0].type, replicate: it[0].replicate] }).bytes.encodeBase64().toString() },
                                                                                                                       ^^
  ```

- Warning: `workflows/deepmutscan.nf:230:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_ec.map { rows -> rows.collect { it[1] } },
                                             ^^
  ```

- Warning: `workflows/deepmutscan.nf:333:68`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
            .mix(CALCULATE_FITNESS.out.dimsum_dir.flatten().filter { it.name == 'report.html' }.map { f -> [['report', 'dimsum', 'DiMSum'], f] })
                                                                     ^^
  ```

- Warning: `workflows/deepmutscan.nf:341:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              def ch_structure = Channel
                                 ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:439:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def manifest = rows.collect { [kind: it[0][0], group: it[0][1], name: it[0][2]] }
                                                   ^^
  ```

- Warning: `workflows/deepmutscan.nf:439:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def manifest = rows.collect { [kind: it[0][0], group: it[0][1], name: it[0][2]] }
                                                                    ^^
  ```

- Warning: `workflows/deepmutscan.nf:439:83`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def manifest = rows.collect { [kind: it[0][0], group: it[0][1], name: it[0][2]] }
                                                                                    ^^
  ```

- Warning: `workflows/deepmutscan.nf:442:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  rows.collect { it[1] },
                                 ^^
  ```
