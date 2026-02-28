# Nextflow lint results

- Generated: 2026-02-28T00:18:40.158085308Z
- Nextflow version: 26.01.1-edge
- Summary: 50 errors, 90 warnings

## :x: Errors

- Error: `conf/test.config:30:24`: `nnk_nns` is not defined

  ```nextflow
      mutagenesis_type = nnk_nns
                         ^^^^^^^
  ```

- Error: `modules/local/fitness/fitness_standard.nf:76:15`: `sample` is already declared

  ```nextflow
      tuple val(sample), path(wt_seq)   		      // WT sequence
                ^^^^^^
  ```

- Error: `nextflow.config:324:35`: `manifest` is not defined

  ```nextflow
  \033[0;35m  nf-core/deepmutscan ${manifest.version}\033[0m
                                    ^^^^^^^^
  ```

- Error: `nextflow.config:327:26`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                           ^^^^^^^^
  ```

- Error: `nextflow.config:327:69`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                      ^^^^^^^^
  ```

- Error: `nextflow.config:327:186`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                                                                                                                                           ^^^^^^^^
  ```

- Error: `nextflow.config:336:22`: `validation` is not defined

  ```nextflow
          beforeText = validation.help.beforeText
                       ^^^^^^^^^^
  ```

- Error: `nextflow.config:337:21`: `validation` is not defined

  ```nextflow
          afterText = validation.help.afterText
                      ^^^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:38:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  Channel
  ^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:42:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  Channel
  ^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:45:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  Channel
  ^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:48:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  Channel
  ^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:51:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  Channel
  ^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:54:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  Channel
  ^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:57:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  Channel
  ^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:60:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  Channel
  ^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:63:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  Channel
  ^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:142:9`: `ch_fasta` is not defined

  ```nextflow
          ch_fasta
          ^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:154:26`: `ch_fasta` is not defined

  ```nextflow
      ch_fasta_broadcast = ch_fasta
                           ^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:174:31`: `ch_fasta` is not defined

  ```nextflow
      ch_fasta_path_broadcast = ch_fasta
                                ^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:184:26`: `ch_fasta` is not defined

  ```nextflow
      ch_fasta_for_gatk  = ch_fasta.combine(PREMERGE.out.bam).map { it[1] }		// path -- N
                           ^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:186:26`: `reading_frame_ch` is not defined

  ```nextflow
      ch_rf_for_gatk     = reading_frame_ch.combine(PREMERGE.out.bam).map { it[0] }	// val  -- N
                           ^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:188:26`: `min_counts_ch` is not defined

  ```nextflow
      ch_min_for_gatk    = min_counts_ch.combine(PREMERGE.out.bam).map { it[0] }		// val  -- N
                           ^^^^^^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:198:5`: `ch_fasta` is not defined

  ```nextflow
      ch_fasta,
      ^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:199:5`: `reading_frame_ch` is not defined

  ```nextflow
      reading_frame_ch
      ^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:204:5`: `ch_fasta` is not defined

  ```nextflow
      ch_fasta,
      ^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:205:5`: `reading_frame_ch` is not defined

  ```nextflow
      reading_frame_ch,			// pos_range (as val)
      ^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:206:5`: `mutagenesis_type_ch` is not defined

  ```nextflow
      mutagenesis_type_ch,		// mutagenesis_type (as val)
      ^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:207:5`: `custom_codon_library_ch` is not defined

  ```nextflow
      custom_codon_library_ch		// custom_codon_library (as path)
      ^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:218:32`: `fanout` is not defined

  ```nextflow
      ch_possible_mut_for_proc = fanout( DMSANALYSIS_POSSIBLE_MUTATIONS.out.possible_mutations.map { it[1] } )
                                 ^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:219:32`: `fanout` is not defined

  ```nextflow
      ch_aa_seq_for_proc       = fanout( DMSANALYSIS_AASEQ.out.aa_seq.map { it[1] } )
                                 ^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:220:32`: `fanout` is not defined

  ```nextflow
      ch_min_counts_for_proc   = fanout( min_counts_ch )
                                 ^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:220:40`: `min_counts_ch` is not defined

  ```nextflow
      ch_min_counts_for_proc   = fanout( min_counts_ch )
                                         ^^^^^^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:239:38`: `fanoutTo` is not defined

  ```nextflow
      min_counts_for_cov_ch          = fanoutTo(variantCounts_for_heatmaps_ch, min_counts_ch)
                                       ^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:239:78`: `min_counts_ch` is not defined

  ```nextflow
      min_counts_for_cov_ch          = fanoutTo(variantCounts_for_heatmaps_ch, min_counts_ch)
                                                                               ^^^^^^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:242:38`: `fanoutTo` is not defined

  ```nextflow
      min_counts_for_heatmap_ch      = fanoutTo(variantCounts_for_heatmaps_ch, min_counts_ch)
                                       ^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:242:78`: `min_counts_ch` is not defined

  ```nextflow
      min_counts_for_heatmap_ch      = fanoutTo(variantCounts_for_heatmaps_ch, min_counts_ch)
                                                                               ^^^^^^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:245:38`: `fanoutTo` is not defined

  ```nextflow
      aa_seq_for_bias_ch             = fanoutTo(variantCounts_filtered_by_library_ch, DMSANALYSIS_AASEQ.out.aa_seq.map { it[1] })
                                       ^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:246:38`: `fanoutTo` is not defined

  ```nextflow
      sliding_window_size_N          = fanoutTo(variantCounts_filtered_by_library_ch, sliding_window_size_ch)
                                       ^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:246:85`: `sliding_window_size_ch` is not defined

  ```nextflow
      sliding_window_size_N          = fanoutTo(variantCounts_filtered_by_library_ch, sliding_window_size_ch)
                                                                                      ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:247:38`: `fanoutTo` is not defined

  ```nextflow
      aimed_cov_N                    = fanoutTo(variantCounts_filtered_by_library_ch, aimed_cov_ch)
                                       ^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:247:85`: `aimed_cov_ch` is not defined

  ```nextflow
      aimed_cov_N                    = fanoutTo(variantCounts_filtered_by_library_ch, aimed_cov_ch)
                                                                                      ^^^^^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:250:38`: `fanoutTo` is not defined

  ```nextflow
      possible_mutations_N           = fanoutTo(variantCounts_filtered_by_library_ch, DMSANALYSIS_POSSIBLE_MUTATIONS.out.possible_mutations.map { it[1] })
                                       ^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:251:38`: `fanoutTo` is not defined

  ```nextflow
      min_counts_for_seqdepth_ch     = fanoutTo(variantCounts_filtered_by_library_ch, min_counts_ch)
                                       ^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:251:85`: `min_counts_ch` is not defined

  ```nextflow
      min_counts_for_seqdepth_ch     = fanoutTo(variantCounts_filtered_by_library_ch, min_counts_ch)
                                                                                      ^^^^^^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:289:31`: `ch_fasta` is not defined

  ```nextflow
      ch_fasta_for_fitness    = ch_fasta.combine(variantCounts_filtered_by_library_ch).map { it[1] }		// path(fasta) -- N
                                ^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:290:31`: `reading_frame_ch` is not defined

  ```nextflow
      ch_rf_for_fitness       = reading_frame_ch.combine(variantCounts_filtered_by_library_ch).map { it[0] }	// val(range) -- N
                                ^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:304:13`: `ch_samplesheet_csv` is not defined

  ```nextflow
              ch_samplesheet_csv,                   // Pfad zum Samplesheet
              ^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:305:13`: `ch_fasta` is not defined

  ```nextflow
              ch_fasta,                             // Das originale Fasta Tuple
              ^^^^^^^^
  ```

- Error: `workflows/deepmutscan.nf:306:13`: `reading_frame_ch` is not defined

  ```nextflow
              reading_frame_ch,                     // Reading frame value channel
              ^^^^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `modules/local/bamprocessing/bamfilteringdms.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/bamprocessing/bamfilteringdms.nf:23:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/bamprocessing/bamfilteringdms.nf:39:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/bamprocessing/premerge.nf:41:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/fitness/fitness_standard.nf:75:15`: Variable was declared but not used

  ```nextflow
      tuple val(sample), path(fitness_estimation_tsv)   // from FITNESS_CALCULATION
                ^^^^^^
  ```

- Warning: `modules/local/gatk/saturationmutagenesis.nf:23:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/gatk/saturationmutagenesis.nf:51:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `nextflow.config:327:129`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                                                                                  ^^
  ```

- Warning: `subworkflows/local/calculatefitness.nf:30:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/calculatefitness.nf:43:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def metas   = pairs.collect { it[0] }
                                            ^^
  ```

- Warning: `subworkflows/local/calculatefitness.nf:44:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def inputs  = pairs.findAll { it[0].type == 'input'  }.sort { it[0].replicate }.collect { it[1] }
                                            ^^
  ```

- Warning: `subworkflows/local/calculatefitness.nf:44:75`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def inputs  = pairs.findAll { it[0].type == 'input'  }.sort { it[0].replicate }.collect { it[1] }
                                                                            ^^
  ```

- Warning: `subworkflows/local/calculatefitness.nf:44:103`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def inputs  = pairs.findAll { it[0].type == 'input'  }.sort { it[0].replicate }.collect { it[1] }
                                                                                                        ^^
  ```

- Warning: `subworkflows/local/calculatefitness.nf:45:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def outputs = pairs.findAll { it[0].type == 'output' }.sort { it[0].replicate }.collect { it[1] }
                                            ^^
  ```

- Warning: `subworkflows/local/calculatefitness.nf:45:75`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def outputs = pairs.findAll { it[0].type == 'output' }.sort { it[0].replicate }.collect { it[1] }
                                                                            ^^
  ```

- Warning: `subworkflows/local/calculatefitness.nf:45:103`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def outputs = pairs.findAll { it[0].type == 'output' }.sort { it[0].replicate }.collect { it[1] }
                                                                                                        ^^
  ```

- Warning: `subworkflows/local/calculatefitness.nf:48:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { smeta, metas, ins, outs -> ins && outs }
                    ^^^^^
  ```

- Warning: `subworkflows/local/calculatefitness.nf:48:26`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { smeta, metas, ins, outs -> ins && outs }
                           ^^^^^
  ```

- Warning: `subworkflows/local/calculatefitness.nf:61:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_fasta_path = ch_fasta.map { it[1] } // strip meta
                                         ^^
  ```

- Warning: `subworkflows/local/calculatefitness.nf:65:69`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta_path.combine(MERGE_COUNTS.out.merged_counts).map { it[0] },
                                                                      ^^
  ```

- Warning: `subworkflows/local/calculatefitness.nf:66:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          val_reading_frame.combine(MERGE_COUNTS.out.merged_counts).map { it[0] }
                                                                          ^^
  ```

- Warning: `subworkflows/local/calculatefitness.nf:82:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { key, smp, counts, wt -> tuple(smp, counts, wt) }
                 ^^^
  ```

- Warning: `subworkflows/local/calculatefitness.nf:87:16`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { it[0] }
                 ^^
  ```

- Warning: `subworkflows/local/calculatefitness.nf:90:61`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def ch_run_counts_d = ch_counts_wt_d.map { smp, counts, wt -> tuple(smp, counts) }
                                                              ^^
  ```

- Warning: `subworkflows/local/calculatefitness.nf:91:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def ch_run_wt_d     = ch_counts_wt_d.map { smp, counts, wt -> wt }
                                                 ^^^
  ```

- Warning: `subworkflows/local/calculatefitness.nf:91:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def ch_run_wt_d     = ch_counts_wt_d.map { smp, counts, wt -> wt }
                                                      ^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_deepmutscan_pipeline/main.nf:31:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_deepmutscan_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_deepmutscan_pipeline/main.nf:38:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_deepmutscan_pipeline/main.nf:75:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:101:98`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      return ch_versions.unique().map { version -> processVersionsFromYAML(version) }.unique().mix(Channel.of(workflowVersionToYAML()))
                                                                                                   ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:38:1`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  Channel
  ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:41:12`: Variable was declared but not used

  ```nextflow
      .set { ch_fasta }
             ^^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:42:1`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  Channel
  ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:44:12`: Variable was declared but not used

  ```nextflow
      .set { reading_frame_ch }
             ^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:45:1`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  Channel
  ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:47:12`: Variable was declared but not used

  ```nextflow
      .set { min_counts_ch }
             ^^^^^^^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:48:1`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  Channel
  ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:50:12`: Variable was declared but not used

  ```nextflow
      .set { custom_codon_library_ch }
             ^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:51:1`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  Channel
  ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:53:12`: Variable was declared but not used

  ```nextflow
      .set { mutagenesis_type_ch }
             ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:54:1`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  Channel
  ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:56:12`: Variable was declared but not used

  ```nextflow
      .set { sliding_window_size_ch }
             ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:57:1`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  Channel
  ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:59:12`: Variable was declared but not used

  ```nextflow
      .set { aimed_cov_ch }
             ^^^^^^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:60:1`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  Channel
  ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:62:12`: Variable was declared but not used

  ```nextflow
      .set { run_seqdepth_ch }
             ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:63:1`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  Channel
  ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:65:10`: Variable was declared but not used

  ```nextflow
    .set { ch_samplesheet_csv }
           ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:74:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:75:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:83:68`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(FASTQC.out.zip.collect{it[1]})
                                                                     ^^
  ```

- Warning: `workflows/deepmutscan.nf:101:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_config        = Channel.fromPath(
                                 ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:104:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.fromPath(params.multiqc_config, checkIfExists: true) :
          ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:105:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.empty()
          ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:107:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.fromPath(params.multiqc_logo, checkIfExists: true) :
          ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:108:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.empty()
          ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:112:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_workflow_summary = Channel.value(paramsSummaryMultiqc(summary_params))
                            ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:118:45`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_methods_description                = Channel.value(
                                              ^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:151:15`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        .map { [it[2], it[3]] }
                ^^
  ```

- Warning: `workflows/deepmutscan.nf:151:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        .map { [it[2], it[3]] }
                       ^^
  ```

- Warning: `workflows/deepmutscan.nf:156:15`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        .map { [it[0], it[1]] }
                ^^
  ```

- Warning: `workflows/deepmutscan.nf:156:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        .map { [it[0], it[1]] }
                       ^^
  ```

- Warning: `workflows/deepmutscan.nf:176:14`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
        .map { it[1] }                    // keep only the fasta path (N emissions)
               ^^
  ```

- Warning: `workflows/deepmutscan.nf:184:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_fasta_for_gatk  = ch_fasta.combine(PREMERGE.out.bam).map { it[1] }		// path -- N
                                                                    ^^
  ```

- Warning: `workflows/deepmutscan.nf:186:75`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_rf_for_gatk     = reading_frame_ch.combine(PREMERGE.out.bam).map { it[0] }	// val  -- N
                                                                            ^^
  ```

- Warning: `workflows/deepmutscan.nf:188:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_min_for_gatk    = min_counts_ch.combine(PREMERGE.out.bam).map { it[0] }		// val  -- N
                                                                         ^^
  ```

- Warning: `workflows/deepmutscan.nf:215:9`: Variable was declared but not used

  ```nextflow
      def fanout = { ch_singleton -> ch_singleton.combine(ch_vc).map { it[0] } }
          ^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:215:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def fanout = { ch_singleton -> ch_singleton.combine(ch_vc).map { it[0] } }
                                                                       ^^
  ```

- Warning: `workflows/deepmutscan.nf:218:100`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_possible_mut_for_proc = fanout( DMSANALYSIS_POSSIBLE_MUTATIONS.out.possible_mutations.map { it[1] } )
                                                                                                     ^^
  ```

- Warning: `workflows/deepmutscan.nf:219:75`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_aa_seq_for_proc       = fanout( DMSANALYSIS_AASEQ.out.aa_seq.map { it[1] } )
                                                                            ^^
  ```

- Warning: `workflows/deepmutscan.nf:230:5`: Variable was declared but not used

  ```nextflow
      annotated_variantCounts_ch = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, a) }
      ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:230:102`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      annotated_variantCounts_ch = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, a) }
                                                                                                       ^
  ```

- Warning: `workflows/deepmutscan.nf:230:105`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      annotated_variantCounts_ch = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, a) }
                                                                                                          ^
  ```

- Warning: `workflows/deepmutscan.nf:230:108`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      annotated_variantCounts_ch = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, a) }
                                                                                                             ^
  ```

- Warning: `workflows/deepmutscan.nf:231:109`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      variantCounts_filtered_by_library_ch = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, b) }
                                                                                                              ^
  ```

- Warning: `workflows/deepmutscan.nf:231:115`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      variantCounts_filtered_by_library_ch = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, b) }
                                                                                                                    ^
  ```

- Warning: `workflows/deepmutscan.nf:231:118`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      variantCounts_filtered_by_library_ch = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, b) }
                                                                                                                       ^
  ```

- Warning: `workflows/deepmutscan.nf:232:107`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      library_completed_variantCounts_ch = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, c) }
                                                                                                            ^
  ```

- Warning: `workflows/deepmutscan.nf:232:110`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      library_completed_variantCounts_ch = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, c) }
                                                                                                               ^
  ```

- Warning: `workflows/deepmutscan.nf:232:116`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      library_completed_variantCounts_ch = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, c) }
                                                                                                                     ^
  ```

- Warning: `workflows/deepmutscan.nf:233:102`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      variantCounts_for_heatmaps_ch = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, d) }
                                                                                                       ^
  ```

- Warning: `workflows/deepmutscan.nf:233:105`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      variantCounts_for_heatmaps_ch = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, d) }
                                                                                                          ^
  ```

- Warning: `workflows/deepmutscan.nf:233:108`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      variantCounts_for_heatmaps_ch = DMSANALYSIS_PROCESS_GATK.out.processed_variantCounts.map { meta, a, b, c, d -> tuple(meta, d) }
                                                                                                             ^
  ```

- Warning: `workflows/deepmutscan.nf:236:9`: Variable was declared but not used

  ```nextflow
      def fanoutTo = { anchorN, singleton -> singleton.combine(anchorN).map { it[0] } }
          ^^^^^^^^
  ```

- Warning: `workflows/deepmutscan.nf:236:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def fanoutTo = { anchorN, singleton -> singleton.combine(anchorN).map { it[0] } }
                                                                              ^^
  ```

- Warning: `workflows/deepmutscan.nf:245:120`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      aa_seq_for_bias_ch             = fanoutTo(variantCounts_filtered_by_library_ch, DMSANALYSIS_AASEQ.out.aa_seq.map { it[1] })
                                                                                                                         ^^
  ```

- Warning: `workflows/deepmutscan.nf:250:145`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      possible_mutations_N           = fanoutTo(variantCounts_filtered_by_library_ch, DMSANALYSIS_POSSIBLE_MUTATIONS.out.possible_mutations.map { it[1] })
                                                                                                                                                  ^^
  ```

- Warning: `workflows/deepmutscan.nf:289:92`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_fasta_for_fitness    = ch_fasta.combine(variantCounts_filtered_by_library_ch).map { it[1] }		// path(fasta) -- N
                                                                                             ^^
  ```

- Warning: `workflows/deepmutscan.nf:290:100`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_rf_for_fitness       = reading_frame_ch.combine(variantCounts_filtered_by_library_ch).map { it[0] }	// val(range) -- N
                                                                                                     ^^
  ```
