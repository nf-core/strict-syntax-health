# Nextflow lint results

- Generated: 2026-07-17T00:29:21.968582093Z
- Nextflow version: 26.07.0-edge
- Summary: 104 warnings

## :warning: Warnings

- Warning: `modules/local/bamprocessing/bam_filter/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/bamprocessing/bam_filter/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/bamprocessing/bam_filter/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/bamprocessing/premerge/main.nf:41:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:31:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:45:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def inputs  = pairs.findAll { it[0].type == 'input'  }.sort { it[0].replicate }.collect { it[1] }
                                            ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:45:75`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def inputs  = pairs.findAll { it[0].type == 'input'  }.sort { it[0].replicate }.collect { it[1] }
                                                                            ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:45:103`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def inputs  = pairs.findAll { it[0].type == 'input'  }.sort { it[0].replicate }.collect { it[1] }
                                                                                                        ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:46:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def outputs = pairs.findAll { it[0].type == 'output' }.sort { it[0].replicate }.collect { it[1] }
                                            ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:46:75`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def outputs = pairs.findAll { it[0].type == 'output' }.sort { it[0].replicate }.collect { it[1] }
                                                                            ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:46:103`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def outputs = pairs.findAll { it[0].type == 'output' }.sort { it[0].replicate }.collect { it[1] }
                                                                                                        ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:49:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { smeta, ins, outs -> ins && outs }
                    ^^^^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:62:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_fasta_path = ch_fasta.map { it[1] } // strip meta
                                         ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:66:69`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta_path.combine(MERGE_COUNTS.out.merged_counts).map { it[0] },
                                                                      ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:67:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          val_reading_frame.combine(MERGE_COUNTS.out.merged_counts).map { it[0] }
                                                                          ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:83:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { key, smp, counts, wt -> tuple(smp, counts, wt) }
                 ^^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:88:16`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { it[0] }
                 ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:91:61`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def ch_run_counts_d = ch_counts_wt_d.map { smp, counts, wt -> tuple(smp, counts) }
                                                              ^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:92:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def ch_run_wt_d     = ch_counts_wt_d.map { smp, counts, wt -> wt }
                                                 ^^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:92:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def ch_run_wt_d     = ch_counts_wt_d.map { smp, counts, wt -> wt }
                                                      ^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_deepmutscan_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_deepmutscan_pipeline/main.nf:36:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_deepmutscan_pipeline/main.nf:106:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:54:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_versions = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:55:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_multiqc_files = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:58:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_fasta = Channel
                     ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:62:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def reading_frame_ch        = Channel.value(params.reading_frame)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:63:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def min_counts_ch           = Channel.value(params.min_counts)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:64:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def custom_codon_library_ch = Channel.value(params.custom_codon_library)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:65:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def mutagenesis_type_ch     = Channel.value(params.mutagenesis_type)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:66:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def sliding_window_size_ch  = Channel.value(params.sliding_window_size)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:67:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def aimed_cov_ch            = Channel.value(params.aimed_cov)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:68:9`: Variable was declared but not used

  ```nextflow
      def run_seqdepth_ch         = Channel.value(params.run_seqdepth)
          ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:68:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def run_seqdepth_ch         = Channel.value(params.run_seqdepth)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:69:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def base_qual_ch            = Channel.value(params.base_qual)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:70:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def min_flank_ch            = Channel.value(params.min_flank)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:73:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_samplesheet_csv      = Channel.fromPath(params.input, checkIfExists: true)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:86:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  pairs.groupBy { it[0] }.each { sample, rows ->
                                  ^^
  ```

- Warning: `workflows/deepmutscan.nf:87:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      def types = rows.collect { it[1] }
                                                 ^^
  ```

- Warning: `workflows/deepmutscan.nf:88:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      if (types.any { it != 'wildtype' } && !types.contains('wildtype')) {
                                      ^^
  ```

- Warning: `workflows/deepmutscan.nf:133:15`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        .map { [it[2], it[3]] }
                ^^
  ```

- Warning: `workflows/deepmutscan.nf:133:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        .map { [it[2], it[3]] }
                       ^^
  ```

- Warning: `workflows/deepmutscan.nf:138:15`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        .map { [it[0], it[1]] }
                ^^
  ```

- Warning: `workflows/deepmutscan.nf:138:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        .map { [it[0], it[1]] }
                       ^^
  ```

- Warning: `workflows/deepmutscan.nf:158:14`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        .map { it[1] }                    // keep only the fasta path (N emissions)
               ^^
  ```

- Warning: `workflows/deepmutscan.nf:169:7`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
        Channel.value('')                                        // index_format '' -> index separately
        ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:177:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_fasta_for_counts = ch_fasta.combine(ch_sorted_indexed).map { it[1] }          // path -- N
                                                                          ^^
  ```

- Warning: `workflows/deepmutscan.nf:178:81`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_rf_for_counts    = reading_frame_ch.combine(ch_sorted_indexed).map { it[0] }  // val  -- N
                                                                                  ^^
  ```

- Warning: `workflows/deepmutscan.nf:179:78`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_min_for_counts   = min_counts_ch.combine(ch_sorted_indexed).map { it[0] }     // val  -- N
                                                                               ^^
  ```

- Warning: `workflows/deepmutscan.nf:180:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_bq_for_counts    = base_qual_ch.combine(ch_sorted_indexed).map { it[0] }      // val  -- N
                                                                              ^^
  ```

- Warning: `workflows/deepmutscan.nf:181:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_flank_for_counts = min_flank_ch.combine(ch_sorted_indexed).map { it[0] }      // val  -- N
                                                                              ^^
  ```

- Warning: `workflows/deepmutscan.nf:211:96`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_possible_mut_for_proc = DMSANALYSIS_POSSIBLE_MUTATIONS.out.possible_mutations.map { it[1] }.combine(ch_vc).map { it[0] }
                                                                                                 ^^
  ```

- Warning: `workflows/deepmutscan.nf:211:125`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_possible_mut_for_proc = DMSANALYSIS_POSSIBLE_MUTATIONS.out.possible_mutations.map { it[1] }.combine(ch_vc).map { it[0] }
                                                                                                                              ^^
  ```

- Warning: `workflows/deepmutscan.nf:212:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_aa_seq_for_proc       = DMSANALYSIS_AASEQ.out.aa_seq.map { it[1] }.combine(ch_vc).map { it[0] }
                                                                        ^^
  ```

- Warning: `workflows/deepmutscan.nf:212:100`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_aa_seq_for_proc       = DMSANALYSIS_AASEQ.out.aa_seq.map { it[1] }.combine(ch_vc).map { it[0] }
                                                                                                     ^^
  ```

- Warning: `workflows/deepmutscan.nf:213:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_min_counts_for_proc   = min_counts_ch.combine(ch_vc).map { it[0] }
                                                                        ^^
  ```

- Warning: `workflows/deepmutscan.nf:223:9`: Variable was declared but not used

  ```nextflow
      def annotated_variantCounts_ch           = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, a) }
          ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:223:126`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def annotated_variantCounts_ch           = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, a) }
                                                                                                                               ^
  ```

- Warning: `workflows/deepmutscan.nf:223:129`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def annotated_variantCounts_ch           = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, a) }
                                                                                                                                  ^
  ```

- Warning: `workflows/deepmutscan.nf:223:132`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def annotated_variantCounts_ch           = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, a) }
                                                                                                                                     ^
  ```

- Warning: `workflows/deepmutscan.nf:224:123`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_filtered_by_library_ch = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, b) }
                                                                                                                            ^
  ```

- Warning: `workflows/deepmutscan.nf:224:129`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_filtered_by_library_ch = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, b) }
                                                                                                                                  ^
  ```

- Warning: `workflows/deepmutscan.nf:224:132`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_filtered_by_library_ch = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, b) }
                                                                                                                                     ^
  ```

- Warning: `workflows/deepmutscan.nf:225:123`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def library_completed_variantCounts_ch   = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, c) }
                                                                                                                            ^
  ```

- Warning: `workflows/deepmutscan.nf:225:126`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def library_completed_variantCounts_ch   = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, c) }
                                                                                                                               ^
  ```

- Warning: `workflows/deepmutscan.nf:225:132`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def library_completed_variantCounts_ch   = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, c) }
                                                                                                                                     ^
  ```

- Warning: `workflows/deepmutscan.nf:226:123`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_for_heatmaps_ch        = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, d) }
                                                                                                                            ^
  ```

- Warning: `workflows/deepmutscan.nf:226:126`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_for_heatmaps_ch        = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, d) }
                                                                                                                               ^
  ```

- Warning: `workflows/deepmutscan.nf:226:129`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_for_heatmaps_ch        = DMSANALYSIS_PROCESS_VARIANT_COUNTS.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, d) }
                                                                                                                                  ^
  ```

- Warning: `workflows/deepmutscan.nf:236:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        def aa_seq_for_ec  = DMSANALYSIS_AASEQ.out.aa_seq.map { it[1] }.combine(ch_fd_in).map { it[0] }
                                                                ^^
  ```

- Warning: `workflows/deepmutscan.nf:236:95`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        def aa_seq_for_ec  = DMSANALYSIS_AASEQ.out.aa_seq.map { it[1] }.combine(ch_fd_in).map { it[0] }
                                                                                                ^^
  ```

- Warning: `workflows/deepmutscan.nf:237:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        def min_for_ec     = min_counts_ch.combine(ch_fd_in).map { it[0] }
                                                                   ^^
  ```

- Warning: `workflows/deepmutscan.nf:240:121`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_filtered_by_library_ch = DMSANALYSIS_ERROR_CORRECTION_FALSE_DOUBLES.out.corrected.map { meta, filt, heat, comp -> tuple(meta, filt) }
                                                                                                                          ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:240:127`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_filtered_by_library_ch = DMSANALYSIS_ERROR_CORRECTION_FALSE_DOUBLES.out.corrected.map { meta, filt, heat, comp -> tuple(meta, filt) }
                                                                                                                                ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:241:115`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_for_heatmaps_ch        = DMSANALYSIS_ERROR_CORRECTION_FALSE_DOUBLES.out.corrected.map { meta, filt, heat, comp -> tuple(meta, heat) }
                                                                                                                    ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:241:127`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_for_heatmaps_ch        = DMSANALYSIS_ERROR_CORRECTION_FALSE_DOUBLES.out.corrected.map { meta, filt, heat, comp -> tuple(meta, heat) }
                                                                                                                                ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:242:115`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        library_completed_variantCounts_ch   = DMSANALYSIS_ERROR_CORRECTION_FALSE_DOUBLES.out.corrected.map { meta, filt, heat, comp -> tuple(meta, comp) }
                                                                                                                    ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:242:121`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        library_completed_variantCounts_ch   = DMSANALYSIS_ERROR_CORRECTION_FALSE_DOUBLES.out.corrected.map { meta, filt, heat, comp -> tuple(meta, comp) }
                                                                                                                          ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:247:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        def wt_ch     = filt_comp.filter { meta, f, c -> meta.type == 'wildtype' }.map { meta, f, c -> tuple(meta.sample, f) }
                                                 ^
  ```

- Warning: `workflows/deepmutscan.nf:247:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        def wt_ch     = filt_comp.filter { meta, f, c -> meta.type == 'wildtype' }.map { meta, f, c -> tuple(meta.sample, f) }
                                                    ^
  ```

- Warning: `workflows/deepmutscan.nf:247:97`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        def wt_ch     = filt_comp.filter { meta, f, c -> meta.type == 'wildtype' }.map { meta, f, c -> tuple(meta.sample, f) }
                                                                                                  ^
  ```

- Warning: `workflows/deepmutscan.nf:248:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        def tgt_ch    = filt_comp.filter { meta, f, c -> meta.type != 'wildtype' }.map { meta, f, c -> tuple(meta.sample, meta, f, c) }
                                                 ^
  ```

- Warning: `workflows/deepmutscan.nf:248:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        def tgt_ch    = filt_comp.filter { meta, f, c -> meta.type != 'wildtype' }.map { meta, f, c -> tuple(meta.sample, meta, f, c) }
                                                    ^
  ```

- Warning: `workflows/deepmutscan.nf:250:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        def aa_seq_for_ec = DMSANALYSIS_AASEQ.out.aa_seq.map { it[1] }.combine(ch_wt_in).map { it[0] }
                                                               ^^
  ```

- Warning: `workflows/deepmutscan.nf:250:94`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        def aa_seq_for_ec = DMSANALYSIS_AASEQ.out.aa_seq.map { it[1] }.combine(ch_wt_in).map { it[0] }
                                                                                               ^^
  ```

- Warning: `workflows/deepmutscan.nf:251:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        def min_for_ec    = min_counts_ch.combine(ch_wt_in).map { it[0] }
                                                                  ^^
  ```

- Warning: `workflows/deepmutscan.nf:254:116`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_filtered_by_library_ch = DMSANALYSIS_ERROR_CORRECTION_WILDTYPE.out.corrected.map { meta, filt, heat, comp -> tuple(meta, filt) }
                                                                                                                     ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:254:122`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_filtered_by_library_ch = DMSANALYSIS_ERROR_CORRECTION_WILDTYPE.out.corrected.map { meta, filt, heat, comp -> tuple(meta, filt) }
                                                                                                                           ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:255:110`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_for_heatmaps_ch        = DMSANALYSIS_ERROR_CORRECTION_WILDTYPE.out.corrected.map { meta, filt, heat, comp -> tuple(meta, heat) }
                                                                                                               ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:255:122`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        variantCounts_for_heatmaps_ch        = DMSANALYSIS_ERROR_CORRECTION_WILDTYPE.out.corrected.map { meta, filt, heat, comp -> tuple(meta, heat) }
                                                                                                                           ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:256:110`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        library_completed_variantCounts_ch   = DMSANALYSIS_ERROR_CORRECTION_WILDTYPE.out.corrected.map { meta, filt, heat, comp -> tuple(meta, comp) }
                                                                                                               ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:256:116`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
        library_completed_variantCounts_ch   = DMSANALYSIS_ERROR_CORRECTION_WILDTYPE.out.corrected.map { meta, filt, heat, comp -> tuple(meta, comp) }
                                                                                                                     ^^^^
  ```

- Warning: `workflows/deepmutscan.nf:273:101`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def min_counts_for_cov_ch          = min_counts_ch.combine(variantCounts_for_heatmaps_ch).map { it[0] }
                                                                                                      ^^
  ```

- Warning: `workflows/deepmutscan.nf:274:101`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def min_counts_for_heatmap_ch      = min_counts_ch.combine(variantCounts_for_heatmaps_ch).map { it[0] }
                                                                                                      ^^
  ```

- Warning: `workflows/deepmutscan.nf:277:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def aa_seq_for_bias_ch             = DMSANALYSIS_AASEQ.out.aa_seq.map { it[1] }.combine(variantCounts_filtered_by_library_ch).map { it[0] }
                                                                              ^^
  ```

- Warning: `workflows/deepmutscan.nf:277:137`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def aa_seq_for_bias_ch             = DMSANALYSIS_AASEQ.out.aa_seq.map { it[1] }.combine(variantCounts_filtered_by_library_ch).map { it[0] }
                                                                                                                                          ^^
  ```

- Warning: `workflows/deepmutscan.nf:278:117`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def sliding_window_size_N          = sliding_window_size_ch.combine(variantCounts_filtered_by_library_ch).map { it[0] }
                                                                                                                      ^^
  ```

- Warning: `workflows/deepmutscan.nf:279:107`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def aimed_cov_N                    = aimed_cov_ch.combine(variantCounts_filtered_by_library_ch).map { it[0] }
                                                                                                            ^^
  ```

- Warning: `workflows/deepmutscan.nf:282:102`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def possible_mutations_N           = DMSANALYSIS_POSSIBLE_MUTATIONS.out.possible_mutations.map { it[1] }.combine(variantCounts_filtered_by_library_ch).map { it[0] }
                                                                                                       ^^
  ```

- Warning: `workflows/deepmutscan.nf:282:162`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def possible_mutations_N           = DMSANALYSIS_POSSIBLE_MUTATIONS.out.possible_mutations.map { it[1] }.combine(variantCounts_filtered_by_library_ch).map { it[0] }
                                                                                                                                                                   ^^
  ```

- Warning: `workflows/deepmutscan.nf:283:108`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def min_counts_for_seqdepth_ch     = min_counts_ch.combine(variantCounts_filtered_by_library_ch).map { it[0] }
                                                                                                             ^^
  ```

- Warning: `workflows/deepmutscan.nf:321:96`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_fasta_for_fitness    = ch_fasta.combine(variantCounts_filtered_by_library_ch).map { it[1] }      // path(fasta) -- N
                                                                                                 ^^
  ```

- Warning: `workflows/deepmutscan.nf:322:104`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_rf_for_fitness       = reading_frame_ch.combine(variantCounts_filtered_by_library_ch).map { it[0] }  // val(range) -- N
                                                                                                         ^^
  ```

- Warning: `workflows/deepmutscan.nf:351:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              def ch_structure = Channel
                                 ^^^^^^^
  ```
