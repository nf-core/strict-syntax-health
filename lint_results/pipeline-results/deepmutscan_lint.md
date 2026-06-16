# Nextflow lint results

- Generated: 2026-06-16T00:50:42.571800483Z
- Nextflow version: 26.04.3
- Summary: 80 warnings

## :warning: Warnings

- Warning: `main.nf:58:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = DEEPMUTSCAN.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

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

- Warning: `modules/local/bamprocessing/bam_filter/main.nf:39:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/bamprocessing/premerge/main.nf:41:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/gatk/saturationmutagenesis/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/gatk/saturationmutagenesis/main.nf:51:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:31:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:44:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def metas   = pairs.collect { it[0] }
                                            ^^
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
          .filter { smeta, metas, ins, outs -> ins && outs }
                    ^^^^^
  ```

- Warning: `subworkflows/local/calculate_fitness/main.nf:49:26`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { smeta, metas, ins, outs -> ins && outs }
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

- Warning: `workflows/deepmutscan.nf:48:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_versions = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:49:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_multiqc_files = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:52:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_fasta = Channel
                     ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:56:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def reading_frame_ch        = Channel.value(params.reading_frame)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:57:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def min_counts_ch           = Channel.value(params.min_counts)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:58:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def custom_codon_library_ch = Channel.value(params.custom_codon_library)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:59:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def mutagenesis_type_ch     = Channel.value(params.mutagenesis_type)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:60:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def sliding_window_size_ch  = Channel.value(params.sliding_window_size)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:61:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def aimed_cov_ch            = Channel.value(params.aimed_cov)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:62:9`: Variable was declared but not used

  ```nextflow
      def run_seqdepth_ch         = Channel.value(params.run_seqdepth)
          ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:62:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def run_seqdepth_ch         = Channel.value(params.run_seqdepth)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:65:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_samplesheet_csv      = Channel.fromPath(params.input, checkIfExists: true)
                                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:86:15`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        .map { [it[2], it[3]] }
                ^^
  ```

- Warning: `workflows/deepmutscan.nf:86:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        .map { [it[2], it[3]] }
                       ^^
  ```

- Warning: `workflows/deepmutscan.nf:91:15`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        .map { [it[0], it[1]] }
                ^^
  ```

- Warning: `workflows/deepmutscan.nf:91:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        .map { [it[0], it[1]] }
                       ^^
  ```

- Warning: `workflows/deepmutscan.nf:111:14`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        .map { it[1] }                    // keep only the fasta path (N emissions)
               ^^
  ```

- Warning: `workflows/deepmutscan.nf:119:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_fasta_for_gatk  = ch_fasta.combine(PREMERGE.out.bam).map { it[1] }       // path -- N
                                                                        ^^
  ```

- Warning: `workflows/deepmutscan.nf:121:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_rf_for_gatk     = reading_frame_ch.combine(PREMERGE.out.bam).map { it[0] }   // val  -- N
                                                                                ^^
  ```

- Warning: `workflows/deepmutscan.nf:123:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_min_for_gatk    = min_counts_ch.combine(PREMERGE.out.bam).map { it[0] }      // val  -- N
                                                                             ^^
  ```

- Warning: `workflows/deepmutscan.nf:150:96`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_possible_mut_for_proc = DMSANALYSIS_POSSIBLE_MUTATIONS.out.possible_mutations.map { it[1] }.combine(ch_vc).map { it[0] }
                                                                                                 ^^
  ```

- Warning: `workflows/deepmutscan.nf:150:125`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_possible_mut_for_proc = DMSANALYSIS_POSSIBLE_MUTATIONS.out.possible_mutations.map { it[1] }.combine(ch_vc).map { it[0] }
                                                                                                                              ^^
  ```

- Warning: `workflows/deepmutscan.nf:151:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_aa_seq_for_proc       = DMSANALYSIS_AASEQ.out.aa_seq.map { it[1] }.combine(ch_vc).map { it[0] }
                                                                        ^^
  ```

- Warning: `workflows/deepmutscan.nf:151:100`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_aa_seq_for_proc       = DMSANALYSIS_AASEQ.out.aa_seq.map { it[1] }.combine(ch_vc).map { it[0] }
                                                                                                     ^^
  ```

- Warning: `workflows/deepmutscan.nf:152:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_min_counts_for_proc   = min_counts_ch.combine(ch_vc).map { it[0] }
                                                                        ^^
  ```

- Warning: `workflows/deepmutscan.nf:162:9`: Variable was declared but not used

  ```nextflow
      def annotated_variantCounts_ch           = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, a) }
          ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:162:116`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def annotated_variantCounts_ch           = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, a) }
                                                                                                                     ^
  ```

- Warning: `workflows/deepmutscan.nf:162:119`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def annotated_variantCounts_ch           = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, a) }
                                                                                                                        ^
  ```

- Warning: `workflows/deepmutscan.nf:162:122`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def annotated_variantCounts_ch           = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, a) }
                                                                                                                           ^
  ```

- Warning: `workflows/deepmutscan.nf:163:113`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_filtered_by_library_ch = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, b) }
                                                                                                                  ^
  ```

- Warning: `workflows/deepmutscan.nf:163:119`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_filtered_by_library_ch = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, b) }
                                                                                                                        ^
  ```

- Warning: `workflows/deepmutscan.nf:163:122`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_filtered_by_library_ch = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, b) }
                                                                                                                           ^
  ```

- Warning: `workflows/deepmutscan.nf:164:113`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def library_completed_variantCounts_ch   = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, c) }
                                                                                                                  ^
  ```

- Warning: `workflows/deepmutscan.nf:164:116`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def library_completed_variantCounts_ch   = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, c) }
                                                                                                                     ^
  ```

- Warning: `workflows/deepmutscan.nf:164:122`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def library_completed_variantCounts_ch   = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, c) }
                                                                                                                           ^
  ```

- Warning: `workflows/deepmutscan.nf:165:113`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_for_heatmaps_ch        = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, d) }
                                                                                                                  ^
  ```

- Warning: `workflows/deepmutscan.nf:165:116`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_for_heatmaps_ch        = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, d) }
                                                                                                                     ^
  ```

- Warning: `workflows/deepmutscan.nf:165:119`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def variantCounts_for_heatmaps_ch        = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, d) }
                                                                                                                        ^
  ```

- Warning: `workflows/deepmutscan.nf:168:101`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def min_counts_for_cov_ch          = min_counts_ch.combine(variantCounts_for_heatmaps_ch).map { it[0] }
                                                                                                      ^^
  ```

- Warning: `workflows/deepmutscan.nf:169:101`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def min_counts_for_heatmap_ch      = min_counts_ch.combine(variantCounts_for_heatmaps_ch).map { it[0] }
                                                                                                      ^^
  ```

- Warning: `workflows/deepmutscan.nf:172:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def aa_seq_for_bias_ch             = DMSANALYSIS_AASEQ.out.aa_seq.map { it[1] }.combine(variantCounts_filtered_by_library_ch).map { it[0] }
                                                                              ^^
  ```

- Warning: `workflows/deepmutscan.nf:172:137`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def aa_seq_for_bias_ch             = DMSANALYSIS_AASEQ.out.aa_seq.map { it[1] }.combine(variantCounts_filtered_by_library_ch).map { it[0] }
                                                                                                                                          ^^
  ```

- Warning: `workflows/deepmutscan.nf:173:117`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def sliding_window_size_N          = sliding_window_size_ch.combine(variantCounts_filtered_by_library_ch).map { it[0] }
                                                                                                                      ^^
  ```

- Warning: `workflows/deepmutscan.nf:174:107`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def aimed_cov_N                    = aimed_cov_ch.combine(variantCounts_filtered_by_library_ch).map { it[0] }
                                                                                                            ^^
  ```

- Warning: `workflows/deepmutscan.nf:177:102`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def possible_mutations_N           = DMSANALYSIS_POSSIBLE_MUTATIONS.out.possible_mutations.map { it[1] }.combine(variantCounts_filtered_by_library_ch).map { it[0] }
                                                                                                       ^^
  ```

- Warning: `workflows/deepmutscan.nf:177:162`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def possible_mutations_N           = DMSANALYSIS_POSSIBLE_MUTATIONS.out.possible_mutations.map { it[1] }.combine(variantCounts_filtered_by_library_ch).map { it[0] }
                                                                                                                                                                   ^^
  ```

- Warning: `workflows/deepmutscan.nf:178:108`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def min_counts_for_seqdepth_ch     = min_counts_ch.combine(variantCounts_filtered_by_library_ch).map { it[0] }
                                                                                                             ^^
  ```

- Warning: `workflows/deepmutscan.nf:216:96`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_fasta_for_fitness    = ch_fasta.combine(variantCounts_filtered_by_library_ch).map { it[1] }      // path(fasta) -- N
                                                                                                 ^^
  ```

- Warning: `workflows/deepmutscan.nf:217:104`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_rf_for_fitness       = reading_frame_ch.combine(variantCounts_filtered_by_library_ch).map { it[0] }  // val(range) -- N
                                                                                                         ^^
  ```
