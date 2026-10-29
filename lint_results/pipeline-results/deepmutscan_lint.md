# Nextflow lint results

- Generated: 2026-10-29T00:16:41.951948998Z
- Nextflow version: 26.10.4
- Summary: 115 warnings

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

- Warning: `subworkflows/local/calculate_fitness/main.nf:64:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_fasta_path = ch_fasta.map { it[1] } // strip meta
                                         ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:68:69`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta_path.combine(MERGE_COUNTS.out.merged_counts).map { it[0] },
                                                                      ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:69:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          val_reading_frame.combine(MERGE_COUNTS.out.merged_counts).map { it[0] }
                                                                          ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:85:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { key, smp, counts, wt -> tuple(smp, counts, wt) }
                 ^^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:90:16`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { it[0] }
                 ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:93:61`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def ch_run_counts_d = ch_counts_wt_d.map { smp, counts, wt -> tuple(smp, counts) }
                                                              ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:94:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def ch_run_wt_d     = ch_counts_wt_d.map { smp, counts, wt -> wt }
                                                 ^^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:94:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def ch_run_wt_d     = ch_counts_wt_d.map { smp, counts, wt -> wt }
                                                      ^^^^^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:118:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_dimsum_dir    = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:119:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

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

- Warning: `workflows/deepmutscan.nf:59:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_fasta = Channel
                     ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:69:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def reading_frame_ch        = Channel.value(params.reading_frame)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:70:65`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def custom_codon_library_ch = params.custom_codon_library ? Channel.value(file(params.custom_codon_library, checkIfExists: true)) : Channel.value([])
                                                                  ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:70:137`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def custom_codon_library_ch = params.custom_codon_library ? Channel.value(file(params.custom_codon_library, checkIfExists: true)) : Channel.value([])
                                                                                                                                          ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:71:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def mutagenesis_type_ch     = Channel.value(params.mutagenesis_type)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:72:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def sliding_window_size_ch  = Channel.value(asInt(params.sliding_window_size))
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:73:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def aimed_cov_ch            = Channel.value(asInt(params.aimed_cov))
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:74:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def base_qual_ch            = Channel.value(asInt(params.base_qual))
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:75:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def min_flank_ch            = Channel.value(asInt(params.min_flank))
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:78:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_samplesheet_csv      = Channel.fromPath(params.input, checkIfExists: true)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:140:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_fasta_for_counts = ch_fasta.combine(ch_sorted_indexed).map { it[1] }          // path -- N
                                                                          ^^
  ```

- Warning: `workflows/deepmutscan.nf:141:81`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_rf_for_counts    = reading_frame_ch.combine(ch_sorted_indexed).map { it[0] }  // val  -- N
                                                                                  ^^
  ```

- Warning: `workflows/deepmutscan.nf:142:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_bq_for_counts    = base_qual_ch.combine(ch_sorted_indexed).map { it[0] }      // val  -- N
                                                                              ^^
  ```

- Warning: `workflows/deepmutscan.nf:143:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_flank_for_counts = min_flank_ch.combine(ch_sorted_indexed).map { it[0] }      // val  -- N
                                                                              ^^
  ```

- Warning: `workflows/deepmutscan.nf:172:96`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_possible_mut_for_proc = DMSANALYSIS_POSSIBLE_MUTATIONS.out.possible_mutations.map { it[1] }.combine(ch_vc).map { it[0] }
                                                                                                 ^^
  ```

- Warning: `workflows/deepmutscan.nf:172:125`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_possible_mut_for_proc = DMSANALYSIS_POSSIBLE_MUTATIONS.out.possible_mutations.map { it[1] }.combine(ch_vc).map { it[0] }
                                                                                                                              ^^
  ```

- Warning: `workflows/deepmutscan.nf:173:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_aa_seq_for_proc       = DMSANALYSIS_AASEQ.out.aa_seq.map { it[1] }.combine(ch_vc).map { it[0] }
                                                                        ^^
  ```

- Warning: `workflows/deepmutscan.nf:173:100`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_aa_seq_for_proc       = DMSANALYSIS_AASEQ.out.aa_seq.map { it[1] }.combine(ch_vc).map { it[0] }
                                                                                                     ^^
  ```

- Warning: `workflows/deepmutscan.nf:184:9`: Variable was declared but not used

  ```nextflow
      def annotated_variantCounts_ch           = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, a) }
          ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:184:126`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def annotated_variantCounts_ch           = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, a) }
                                                                                                                               ^
  ```

- Warning: `workflows/deepmutscan.nf:184:129`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def annotated_variantCounts_ch           = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, a) }
                                                                                                                                  ^
  ```

- Warning: `workflows/deepmutscan.nf:184:132`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def annotated_variantCounts_ch           = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, a) }
                                                                                                                                     ^
  ```

- Warning: `workflows/deepmutscan.nf:185:123`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_filtered_by_library_ch = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, b) }
                                                                                                                            ^
  ```

- Warning: `workflows/deepmutscan.nf:185:129`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_filtered_by_library_ch = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, b) }
                                                                                                                                  ^
  ```

- Warning: `workflows/deepmutscan.nf:185:132`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_filtered_by_library_ch = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, b) }
                                                                                                                                     ^
  ```

- Warning: `workflows/deepmutscan.nf:186:123`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def library_completed_variantCounts_ch   = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, c) }
                                                                                                                            ^
  ```

- Warning: `workflows/deepmutscan.nf:186:126`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def library_completed_variantCounts_ch   = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, c) }
                                                                                                                               ^
  ```

- Warning: `workflows/deepmutscan.nf:186:132`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def library_completed_variantCounts_ch   = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, c) }
                                                                                                                                     ^
  ```

- Warning: `workflows/deepmutscan.nf:187:123`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_for_heatmaps_ch        = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, d) }
                                                                                                                            ^
  ```

- Warning: `workflows/deepmutscan.nf:187:126`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_for_heatmaps_ch        = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, d) }
                                                                                                                               ^
  ```

- Warning: `workflows/deepmutscan.nf:187:129`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_for_heatmaps_ch        = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, d) }
                                                                                                                                  ^
  ```

- Warning: `workflows/deepmutscan.nf:197:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        def aa_seq_for_ec  = DMSANALYSIS_AASEQ.out.aa_seq.map { it[1] }.combine(ch_fd_in).map { it[0] }
                                                                ^^
  ```

- Warning: `workflows/deepmutscan.nf:197:95`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        def aa_seq_for_ec  = DMSANALYSIS_AASEQ.out.aa_seq.map { it[1] }.combine(ch_fd_in).map { it[0] }
                                                                                                ^^
  ```

- Warning: `workflows/deepmutscan.nf:201:61`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        def fasta_for_ec   = ch_fasta.combine(ch_fd_in).map { it[1] }
                                                              ^^
  ```

- Warning: `workflows/deepmutscan.nf:207:121`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_filtered_by_library_ch = DMSANALYSIS_ERROR_CORRECTION_FALSE_DOUBLES.out.corrected.map { meta, filt, heat, comp -> tuple(meta, filt) }
                                                                                                                          ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:207:127`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_filtered_by_library_ch = DMSANALYSIS_ERROR_CORRECTION_FALSE_DOUBLES.out.corrected.map { meta, filt, heat, comp -> tuple(meta, filt) }
                                                                                                                                ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:208:115`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_for_heatmaps_ch        = DMSANALYSIS_ERROR_CORRECTION_FALSE_DOUBLES.out.corrected.map { meta, filt, heat, comp -> tuple(meta, heat) }
                                                                                                                    ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:208:127`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_for_heatmaps_ch        = DMSANALYSIS_ERROR_CORRECTION_FALSE_DOUBLES.out.corrected.map { meta, filt, heat, comp -> tuple(meta, heat) }
                                                                                                                                ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:209:115`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        library_completed_variantCounts_ch   = DMSANALYSIS_ERROR_CORRECTION_FALSE_DOUBLES.out.corrected.map { meta, filt, heat, comp -> tuple(meta, comp) }
                                                                                                                    ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:209:121`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        library_completed_variantCounts_ch   = DMSANALYSIS_ERROR_CORRECTION_FALSE_DOUBLES.out.corrected.map { meta, filt, heat, comp -> tuple(meta, comp) }
                                                                                                                          ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:214:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        def wt_ch     = filt_comp.filter { meta, f, c -> meta.type == 'wildtype' }.map { meta, f, c -> tuple(meta.sample, f) }
                                                 ^
  ```

- Warning: `workflows/deepmutscan.nf:214:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        def wt_ch     = filt_comp.filter { meta, f, c -> meta.type == 'wildtype' }.map { meta, f, c -> tuple(meta.sample, f) }
                                                    ^
  ```

- Warning: `workflows/deepmutscan.nf:214:97`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        def wt_ch     = filt_comp.filter { meta, f, c -> meta.type == 'wildtype' }.map { meta, f, c -> tuple(meta.sample, f) }
                                                                                                  ^
  ```

- Warning: `workflows/deepmutscan.nf:215:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        def tgt_ch    = filt_comp.filter { meta, f, c -> meta.type != 'wildtype' }.map { meta, f, c -> tuple(meta.sample, meta, f, c) }
                                                 ^
  ```

- Warning: `workflows/deepmutscan.nf:215:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        def tgt_ch    = filt_comp.filter { meta, f, c -> meta.type != 'wildtype' }.map { meta, f, c -> tuple(meta.sample, meta, f, c) }
                                                    ^
  ```

- Warning: `workflows/deepmutscan.nf:217:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        def aa_seq_for_ec = DMSANALYSIS_AASEQ.out.aa_seq.map { it[1] }.combine(ch_wt_in).map { it[0] }
                                                               ^^
  ```

- Warning: `workflows/deepmutscan.nf:217:94`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        def aa_seq_for_ec = DMSANALYSIS_AASEQ.out.aa_seq.map { it[1] }.combine(ch_wt_in).map { it[0] }
                                                                                               ^^
  ```

- Warning: `workflows/deepmutscan.nf:220:116`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_filtered_by_library_ch = DMSANALYSIS_ERROR_CORRECTION_WILDTYPE.out.corrected.map { meta, filt, heat, comp -> tuple(meta, filt) }
                                                                                                                     ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:220:122`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_filtered_by_library_ch = DMSANALYSIS_ERROR_CORRECTION_WILDTYPE.out.corrected.map { meta, filt, heat, comp -> tuple(meta, filt) }
                                                                                                                           ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:221:110`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_for_heatmaps_ch        = DMSANALYSIS_ERROR_CORRECTION_WILDTYPE.out.corrected.map { meta, filt, heat, comp -> tuple(meta, heat) }
                                                                                                               ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:221:122`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_for_heatmaps_ch        = DMSANALYSIS_ERROR_CORRECTION_WILDTYPE.out.corrected.map { meta, filt, heat, comp -> tuple(meta, heat) }
                                                                                                                           ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:222:110`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        library_completed_variantCounts_ch   = DMSANALYSIS_ERROR_CORRECTION_WILDTYPE.out.corrected.map { meta, filt, heat, comp -> tuple(meta, comp) }
                                                                                                               ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:222:116`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        library_completed_variantCounts_ch   = DMSANALYSIS_ERROR_CORRECTION_WILDTYPE.out.corrected.map { meta, filt, heat, comp -> tuple(meta, comp) }
                                                                                                                     ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:228:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_report_assets = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:240:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_ec.map { rows -> groovy.json.JsonOutput.toJson(rows.collect { [id: it[0].id, type: it[0].type, replicate: it[0].replicate] }).bytes.encodeBase64().toString() },
                                                                                ^^
  ```

- Warning: `workflows/deepmutscan.nf:240:95`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_ec.map { rows -> groovy.json.JsonOutput.toJson(rows.collect { [id: it[0].id, type: it[0].type, replicate: it[0].replicate] }).bytes.encodeBase64().toString() },
                                                                                                ^^
  ```

- Warning: `workflows/deepmutscan.nf:240:118`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_ec.map { rows -> groovy.json.JsonOutput.toJson(rows.collect { [id: it[0].id, type: it[0].type, replicate: it[0].replicate] }).bytes.encodeBase64().toString() },
                                                                                                                       ^^
  ```

- Warning: `workflows/deepmutscan.nf:241:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_ec.map { rows -> rows.collect { it[1] } },
                                             ^^
  ```

- Warning: `workflows/deepmutscan.nf:253:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def aa_seq_for_bias_ch             = DMSANALYSIS_AASEQ.out.aa_seq.map { it[1] }.combine(variantCounts_filtered_by_library_ch).map { it[0] }
                                                                              ^^
  ```

- Warning: `workflows/deepmutscan.nf:253:137`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def aa_seq_for_bias_ch             = DMSANALYSIS_AASEQ.out.aa_seq.map { it[1] }.combine(variantCounts_filtered_by_library_ch).map { it[0] }
                                                                                                                                          ^^
  ```

- Warning: `workflows/deepmutscan.nf:254:117`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def sliding_window_size_N          = sliding_window_size_ch.combine(variantCounts_filtered_by_library_ch).map { it[0] }
                                                                                                                      ^^
  ```

- Warning: `workflows/deepmutscan.nf:255:107`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def aimed_cov_N                    = aimed_cov_ch.combine(variantCounts_filtered_by_library_ch).map { it[0] }
                                                                                                            ^^
  ```

- Warning: `workflows/deepmutscan.nf:258:102`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def possible_mutations_N           = DMSANALYSIS_POSSIBLE_MUTATIONS.out.possible_mutations.map { it[1] }.combine(variantCounts_filtered_by_library_ch).map { it[0] }
                                                                                                       ^^
  ```

- Warning: `workflows/deepmutscan.nf:258:162`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def possible_mutations_N           = DMSANALYSIS_POSSIBLE_MUTATIONS.out.possible_mutations.map { it[1] }.combine(variantCounts_filtered_by_library_ch).map { it[0] }
                                                                                                                                                                   ^^
  ```

- Warning: `workflows/deepmutscan.nf:327:100`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def ch_fasta_for_fitness    = ch_fasta.combine(variantCounts_filtered_by_library_ch).map { it[1] }      // path(fasta) -- N
                                                                                                     ^^
  ```

- Warning: `workflows/deepmutscan.nf:328:108`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def ch_rf_for_fitness       = reading_frame_ch.combine(variantCounts_filtered_by_library_ch).map { it[0] }  // val(range) -- N
                                                                                                             ^^
  ```

- Warning: `workflows/deepmutscan.nf:355:68`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
            .mix(CALCULATE_FITNESS.out.dimsum_dir.flatten().filter { it.name == 'report.html' }.map { f -> [['report', 'dimsum', 'DiMSum'], f] })
                                                                     ^^
  ```

- Warning: `workflows/deepmutscan.nf:363:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              def ch_structure = Channel
                                 ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:461:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.fromPath("${outdir}/pipeline_info/execution_trace_${params.trace_report_suffix}.txt", checkIfExists: false)
          ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:469:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def manifest = rows.collect { [kind: it[0][0], group: it[0][1], name: it[0][2]] }
                                                   ^^
  ```

- Warning: `workflows/deepmutscan.nf:469:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def manifest = rows.collect { [kind: it[0][0], group: it[0][1], name: it[0][2]] }
                                                                    ^^
  ```

- Warning: `workflows/deepmutscan.nf:469:83`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def manifest = rows.collect { [kind: it[0][0], group: it[0][1], name: it[0][2]] }
                                                                                    ^^
  ```

- Warning: `workflows/deepmutscan.nf:472:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  rows.collect { it[1] },
                                 ^^
  ```
