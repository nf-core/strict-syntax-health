# Nextflow lint results

- Generated: 2026-06-30T00:41:48.045288670Z
- Nextflow version: 26.05.0-edge
- Summary: 3 errors, 382 warnings

## :x: Errors

- Error: `tests/config/test_data.config:1:1`: Variable declarations cannot be mixed with config statements

  ```nextflow
  def test_data_dir = "${launchDir}/tests/data/"
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `tests/config/test_data.config:2:1`: Variable declarations cannot be mixed with config statements

  ```nextflow
  def nf_core_modules_data = "https://raw.githubusercontent.com/nf-core/test-datasets/modules/data/"
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `tests/config/test_data.config:4:1`: Try-catch blocks cannot be mixed with config statements

  ```nextflow
  try {
  ^
  ```

## :warning: Warnings

- Warning: `conf/modules/alignment/bam_align.config:48:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      ) { "mapped/${meta.id}/${it}" }
                                               ^^
  ```

- Warning: `conf/modules/alignment/bam_align.config:67:174`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          saveAs: { (params.save_output_as_bam && (params.save_mapped || params.skip_tools && params.skip_tools.split(',').contains('markduplicates'))) ? "mapped/${meta.id}/${it}" : null }
                                                                                                                                                                               ^^
  ```

- Warning: `conf/modules/alignment/bam_align.config:172:209`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { (params.save_bam_mapped || (params.skip_tools && params.skip_tools.split(',').contains('markduplicates'))) && (meta.size * meta.numLanes == 1) ? "mapped/${meta.patient}/${meta.id}/${it}" : null }
                                                                                                                                                                                                                  ^^
  ```

- Warning: `conf/modules/alignment/bam_align.config:184:209`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { (params.save_bam_mapped || (params.skip_tools && params.skip_tools.split(',').contains('markduplicates'))) && (meta.size * meta.numLanes == 1) ? "mapped/${meta.patient}/${meta.id}/${it}" : null }
                                                                                                                                                                                                                  ^^
  ```

- Warning: `conf/modules/gatk4_preprocessing/markduplicates.config:64:145`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { !(params.skip_tools && params.skip_tools.split(',').contains('markduplicates_report')) ? "markduplicates/${meta.id}/${it}" : null}
                                                                                                                                                  ^^
  ```

- Warning: `conf/modules/gatk4_preprocessing/prepare_recalibration.config:25:81`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { meta.num_intervals > 1 ? null : "recal_table/${meta.id}/${it}" }
                                                                                  ^^
  ```

- Warning: `conf/modules/gatk4_preprocessing/recalibrate.config:25:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { meta.num_intervals > 1 ? null : "recalibrated/${meta.id}/${it}" }
                                                                                   ^^
  ```

- Warning: `conf/modules/gatk4_preprocessing/splitncigarreads.config:46:102`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          saveAs: { params.save_bam_mapped ? "realignment/${meta.patient}/${meta.id}/${it}" : null },
                                                                                                       ^^
  ```

- Warning: `conf/modules/variant_calling/mutect2.config:29:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { meta.num_intervals > 1 ? null : "mutect2/${meta.id}/${it}" }
                                                                              ^^
  ```

- Warning: `conf/modules/variant_calling/mutect2.config:101:81`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { meta.num_intervals > 1 ? null : "mutect2/${meta.id}/${it}" }
                                                                                  ^^
  ```

- Warning: `conf/modules/variant_calling/strelka.config:27:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { meta.num_intervals > 1 ? null : "strelka/${meta.id}/${it}" },
                                                                              ^^
  ```

- Warning: `main.nf:60:5`: Variable was declared but not used

  ```nextflow
      versions = Channel.empty()
      ^^^^^^^^
  ```

- Warning: `main.nf:60:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `main.nf:69:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = RNADNAVAR.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/maf2bed/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/merge_maf/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/annotation_cache_initialisation/main.nf:37:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ensemblvep_cache = Channel.value([[id: vep_cache_path_full.baseName], vep_cache_path_full])
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/annotation_cache_initialisation/main.nf:41:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      ensemblvep_cache // channel: [ meta, cache ]
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_align/main.nf:36:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      reports   = Channel.empty()
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_align/main.nf:37:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions  = Channel.empty()
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_align/main.nf:41:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      bam_mapped_rna   = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_align/main.nf:42:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      bam_mapped_dna   = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_align/main.nf:43:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      bam_mapped       = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_align/main.nf:44:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      cram_mapped      = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_align/main.nf:75:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              reports = reports.mix(FASTQC.out.zip.collect{ meta, logs -> logs })
                                                            ^^^^
  ```

- Warning: `subworkflows/local/bam_align/main.nf:196:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          reports           = reports.mix(FASTQ_ALIGN_STAR.out.stats.collect{it[1]}.ifEmpty([]))
                                                                             ^^
  ```

- Warning: `subworkflows/local/bam_align/main.nf:197:80`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          reports           = reports.mix(FASTQ_ALIGN_STAR.out.log_final.collect{it[1]}.ifEmpty([]))
                                                                                 ^^
  ```

- Warning: `subworkflows/local/bam_applybqsr/main.nf:19:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_baserecalibrator/main.nf:21:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_baserecalibrator/main.nf:43:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          single:   it[0].num_intervals <= 1
                    ^^
  ```

- Warning: `subworkflows/local/bam_baserecalibrator/main.nf:44:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          multiple: it[0].num_intervals > 1
                    ^^
  ```

- Warning: `subworkflows/local/bam_baserecalibrator/main.nf:51:5`: Variable was declared but not used

  ```nextflow
      table_bqsr = GATK4_GATHERBQSRREPORTS.out.table.mix(table_to_merge.single.map{ meta, table -> [ meta, table[0] ] })
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_convert_samtools/main.nf:22:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_convert_samtools/main.nf:64:5`: Variable was declared but not used

  ```nextflow
      reads = CAT_FASTQ.out.reads
      ^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:39:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      reports   = Channel.empty()
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:40:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions  = Channel.empty()
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:41:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      cram_variant_calling = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:47:40`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          cram_markduplicates_no_spark = Channel.empty()
                                         ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:57:121`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          cram_for_markduplicates = params.step == 'mapping' || realignment ? bam_mapped : input_sample.map{ meta, input, index -> [ meta, input ] }
                                                                                                                          ^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:61:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          cram_skip_markduplicates = Channel.empty()
                                     ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:70:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      bam:  it[0].data_type == "bam"
                            ^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:71:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      cram: it[0].data_type == "cram"
                            ^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:78:44`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  cram_skip_markduplicates = Channel.empty().mix(input_markduplicates_convert.cram, BAM_TO_CRAM.out.cram)
                                             ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:84:70`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              reports = reports.mix(CRAM_QC_NO_MD.out.reports.collect{ meta, report -> report })
                                                                       ^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:102:75`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              reports = reports.mix(BAM_MARKDUPLICATES.out.reports.collect{ meta, report -> report })
                                                                            ^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:109:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_md_cram_for_restart = Channel.empty().mix(cram_markduplicates_no_spark)
                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:125:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_md_cram_for_restart   = Channel.empty().mix(input_sample)
                                     ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:126:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          cram_skip_markduplicates = Channel.empty().mix(input_sample)
                                     ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:136:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      bam:  it[0].data_type == "bam"
                            ^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:137:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      cram: it[0].data_type == "cram"
                            ^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:140:83`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  input_sncr_convert  = input_sncr_convert.bam.map{ meta, bam, bai, table -> [ meta, bam, bai ] }
                                                                                    ^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:149:41`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  cram_skip_splitncigar = Channel.empty().mix(sncr_cram_from_bam, input_sncr_convert.cram)
                                          ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:159:37`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          cram_splitncigar_no_spark = Channel.empty()
                                      ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:163:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                                  dna:  it[0].status < 2
                                                        ^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:164:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                                  rna:  it[0].status >= 2
                                                        ^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:179:37`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              cram_skip_splitncigar = Channel.empty()
                                      ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:183:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_sncr_cram_for_restart = Channel.empty().mix(cram_splitncigar_no_spark).mix(cram_skip_splitncigar)
                                     ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:187:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_sncr_cram_for_restart = Channel.empty()
                                     ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:199:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  bam: it[0].data_type == "bam"
                       ^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:200:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  cram: it[0].data_type == "cram"
                        ^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:211:48`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_cram_for_bam_baserecalibrator = Channel.empty().mix(ch_cram_for_bam_baserecalibrator, input_prepare_recal_convert.cram)
                                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:222:48`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_cram_for_bam_baserecalibrator = Channel.empty().mix(ch_sncr_cram_for_restart, cram_skip_splitncigar )
                                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:230:38`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_table_bqsr_no_spark = Channel.empty()
                                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:249:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_table_bqsr = Channel.empty().mix(
                              ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:252:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              reports = reports.mix(ch_table_bqsr.collect{ meta, table -> table })
                                                           ^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:271:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  bam:  it[0].data_type == "bam"
                        ^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:272:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  cram: it[0].data_type == "cram"
                        ^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:276:67`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              input_only_table = input_recal_convert.bam.map{ meta, bam, bai, table -> [ meta, table ] }
                                                                    ^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:276:72`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              input_only_table = input_recal_convert.bam.map{ meta, bam, bai, table -> [ meta, table ] }
                                                                         ^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:277:77`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              input_only_bam   = input_recal_convert.bam.map{ meta, bam, bai, table -> [ meta, bam, bai ] }
                                                                              ^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:283:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              cram_applybqsr = Channel.empty().mix(
                               ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:291:45`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              cram_variant_calling_no_spark = Channel.empty()
                                              ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:306:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              cram_variant_calling = Channel.empty().mix(
                                     ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:316:70`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              reports = reports.mix(CRAM_QC_RECAL.out.reports.collect{ meta, report -> report })
                                                                       ^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:328:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              csv_recalibration = Channel.empty()
                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:339:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              cram_variant_calling = Channel.empty().mix(
                                     ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:341:65`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  input_recal_convert.cram.map{ meta, cram, crai, table -> [ meta, cram, crai ] })
                                                                  ^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:345:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              cram_variant_calling = Channel.empty().mix(ch_cram_for_bam_baserecalibrator)
                                     ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:354:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              bam:  it[0].data_type == "bam"
                    ^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:355:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              cram: it[0].data_type == "cram"
                    ^^
  ```

- Warning: `subworkflows/local/bam_gatk_preprocessing/main.nf:364:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          cram_variant_calling = Channel.empty().mix(converted, input_variant_calling_convert.cram)
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_markduplicates/main.nf:18:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_markduplicates/main.nf:19:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      reports  = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_merge_index_samtools/main.nf:15:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_merge_index_samtools/main.nf:36:5`: Variable was declared but not used

  ```nextflow
      bam_bai = bam_all.join(INDEX_MERGE_BAM.out.index, failOnDuplicate: true, failOnMismatch: true)
      ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_splitncigarreads/main.nf:19:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling/main.nf:38:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      reports   = Channel.empty()
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling/main.nf:39:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions  = Channel.empty()
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling/main.nf:42:43`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              cram_variant_calling_pair   = Channel.empty()
                                            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling/main.nf:44:43`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              contamination_table_mutect2 = Channel.empty()
                                            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling/main.nf:45:43`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              segmentation_table_mutect2  = Channel.empty()
                                            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling/main.nf:46:43`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              artifact_priors_mutect2     = Channel.empty()
                                            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling/main.nf:54:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  normal: it[0].status == 0
                          ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling/main.nf:55:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  tumor:  it[0].status >= 1  // DNA and RNA should NOT have same sample id
                          ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling/main.nf:78:13`: Variable was declared but not used

  ```nextflow
              cram_variant_calling_tumor_only = cram_variant_calling_tumor_filtered.transpose().map{ it -> [it[1], it[2], it[3]] }
              ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling/main.nf:137:43`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              vcf_to_normalise            = Channel.empty().mix(BAM_VARIANT_CALLING_SOMATIC.out.vcf_all)
                                            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling/main.nf:138:43`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              contamination_table_mutect2 = Channel.empty().mix(BAM_VARIANT_CALLING_SOMATIC.out.contamination_table_mutect2)
                                            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling/main.nf:139:43`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              segmentation_table_mutect2  = Channel.empty().mix(BAM_VARIANT_CALLING_SOMATIC.out.segmentation_table_mutect2)
                                            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling/main.nf:140:43`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              artifact_priors_mutect2     = Channel.empty().mix(BAM_VARIANT_CALLING_SOMATIC.out.artifact_priors_mutect2)
                                            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling/main.nf:152:84`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          reports = reports.mix(VCF_QC_BCFTOOLS_VCFTOOLS.out.bcftools_stats.collect{ meta, stats -> stats })
                                                                                     ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling/main.nf:153:90`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          reports = reports.mix(VCF_QC_BCFTOOLS_VCFTOOLS.out.vcftools_tstv_counts.collect{ meta, counts -> counts })
                                                                                           ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling/main.nf:154:88`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          reports = reports.mix(VCF_QC_BCFTOOLS_VCFTOOLS.out.vcftools_tstv_qual.collect{ meta, qual -> qual })
                                                                                         ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling/main.nf:155:93`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          reports = reports.mix(VCF_QC_BCFTOOLS_VCFTOOLS.out.vcftools_filter_summary.collect{ meta, summary -> summary })
                                                                                              ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling/main.nf:159:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          cram_variant_calling_pair   = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling/main.nf:160:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          vcf_to_normalise            = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling/main.nf:161:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          contamination_table_mutect2 = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling/main.nf:162:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          segmentation_table_mutect2  = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling/main.nf:163:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          artifact_priors_mutect2     = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_pre_post_processing/main.nf:27:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      dbsnp                           // channel: [optional]  germline_resource
      ^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_pre_post_processing/main.nf:28:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      dbsnp_tbi                       // channel: [optional]  germline_resource_tbi
      ^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_pre_post_processing/main.nf:50:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      reports   = Channel.empty()
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_pre_post_processing/main.nf:51:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions  = Channel.empty()
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_pre_post_processing/main.nf:93:5`: Variable was declared but not used

  ```nextflow
      cram_variant_calling_pair     = BAM_VARIANT_CALLING.out.cram_variant_calling_pair  // use same crams for force calling later
      ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_pre_post_processing/main.nf:95:5`: Variable was declared but not used

  ```nextflow
      contamination                 = BAM_VARIANT_CALLING.out.contamination_table
      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_pre_post_processing/main.nf:96:5`: Variable was declared but not used

  ```nextflow
      segmentation                  = BAM_VARIANT_CALLING.out.segmentation_table
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_pre_post_processing/main.nf:97:5`: Variable was declared but not used

  ```nextflow
      orientation                   = BAM_VARIANT_CALLING.out.artifact_priors
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic/main.nf:20:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      intervals_bed_combined        // channel: [mandatory] intervals/target regions in one file unzipped
      ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic/main.nf:31:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions          = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic/main.nf:33:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_manta         = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic/main.nf:34:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_strelka       = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic/main.nf:35:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_mutect2       = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic/main.nf:36:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_sage          = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic/main.nf:86:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          vcf_strelka = Channel.empty().mix(BAM_VARIANT_CALLING_SOMATIC_STRELKA.out.vcf)
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic/main.nf:119:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          contamination_table_mutect2 = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic/main.nf:120:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          segmentation_table_mutect2  = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic/main.nf:121:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          artifact_priors_mutect2     = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic/main.nf:126:5`: Variable was declared but not used

  ```nextflow
      vcf_all = Channel.empty().mix(
      ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic/main.nf:126:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_all = Channel.empty().mix(
                ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_manta/main.nf:17:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_manta/main.nf:30:5`: Variable was declared but not used

  ```nextflow
      candidate_small_indels_vcf = MANTA_SOMATIC.out.candidate_small_indels_vcf
      ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_manta/main.nf:31:5`: Variable was declared but not used

  ```nextflow
      candidate_small_indels_vcf_tbi = MANTA_SOMATIC.out.candidate_small_indels_vcf_tbi
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_manta/main.nf:32:5`: Variable was declared but not used

  ```nextflow
      candidate_sv_vcf = MANTA_SOMATIC.out.candidate_sv_vcf
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_manta/main.nf:38:5`: Variable was declared but not used

  ```nextflow
      vcf = Channel.empty().mix(diploid_sv_vcf, somatic_sv_vcf).map{ meta, vcf -> [ meta + [ variantcaller:'manta' ], vcf ] }
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_manta/main.nf:38:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf = Channel.empty().mix(diploid_sv_vcf, somatic_sv_vcf).map{ meta, vcf -> [ meta + [ variantcaller:'manta' ], vcf ] }
            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:34:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:44:80`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      germline_resource_pileup     = germline_resource_tbi ? germline_resource : Channel.empty()
                                                                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:45:61`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      germline_resource_pileup_tbi = germline_resource_tbi ?: Channel.empty()
                                                              ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:98:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:99:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:105:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:106:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:112:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:113:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:119:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:120:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:132:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf = Channel.empty().mix(MERGE_MUTECT2.out.vcf, vcf_branch.no_intervals).map{ meta, vcf ->
            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:135:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi = Channel.empty().mix(MERGE_MUTECT2.out.tbi, tbi_branch.no_intervals).map{ meta, tbi->
            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:138:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      stats = Channel.empty().mix(MERGEMUTECTSTATS.out.stats, stats_branch.no_intervals).map{ meta, stats ->
              ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:141:12`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      f1r2 = Channel.empty().mix(f1r2_to_merge, f1r2_branch.no_intervals).map{ meta, f1r2->
             ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:168:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              intervals:    it[0].num_intervals > 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:169:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_intervals: it[0].num_intervals <= 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:175:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              intervals:    it[0].num_intervals > 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:176:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_intervals: it[0].num_intervals <= 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:188:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          pileup_table_tumor  = Channel.empty().mix(GATHERPILEUPSUMMARIES_TUMOR.out.table, pileup_table_tumor_branch.no_intervals).map{meta, table -> [ meta - meta.subMap('normal_id', 'tumor_id', 'num_intervals') + [id:meta.patient], meta.id, table ] }
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:189:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          pileup_table_normal = Channel.empty().mix(GATHERPILEUPSUMMARIES_NORMAL.out.table, pileup_table_normal_branch.no_intervals).map{meta, table -> [ meta - meta.subMap('normal_id', 'tumor_id', 'num_intervals') + [id:meta.patient], meta.id, table ] }
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:206:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_seg_to_filtermutectcalls = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:207:40`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_cont_to_filtermutectcalls = Channel.empty()
                                         ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:240:40`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          artifact_priors              = Channel.empty()
                                         ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:241:40`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_cont_to_filtermutectcalls = Channel.empty()
                                         ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:242:40`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_seg_to_filtermutectcalls  = Channel.empty()
                                         ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:243:40`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          pileup_table_normal          = Channel.empty()
                                         ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:244:40`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          pileup_table_tumor           = Channel.empty()
                                         ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:249:5`: Variable was declared but not used

  ```nextflow
      vcf_filtered = FILTERMUTECTCALLS.out.vcf
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_sage/main.nf:22:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_sage/main.nf:26:50`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      if (!params.sage_ensembl_dir) sage_ensembl = Channel.value([])
                                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_sage/main.nf:28:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          UNTAR_SAGE_ENSEMBL(Channel.fromPath(params.sage_ensembl_dir).collect().map{ it -> [ [ id:it[0].baseName ], it ] })
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_sage/main.nf:32:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          UNZIP_SAGE_ENSEMBL(Channel.fromPath(params.sage_ensembl_dir).collect().map{ it -> [ [ id:it[0].baseName ], it ] })
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_sage/main.nf:36:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          sage_ensembl = Channel.fromPath(params.sage_ensembl_dir).collect().map{ it -> [ [ id:it[0].baseName ], it ] }
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_sage/main.nf:47:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.fromPath(params.sage_high_confidence).collect().map{ it -> [ [ id:it[0].baseName ], it ] },
          ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_sage/main.nf:48:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.fromPath(params.sage_actionable_panel).collect().map{ it -> [ [ id:it[0].baseName ], it ] },
          ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_sage/main.nf:49:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.fromPath(params.sage_known_hotspots).collect().map{ it -> [ [ id:it[0].baseName ], it ] },
          ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_sage/main.nf:57:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_sage/main.nf:58:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_sage/main.nf:74:5`: Variable was declared but not used

  ```nextflow
      vcf = BGZIPTABIX_VC_SAGE.out.output
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_sage/main.nf:78:26`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta, vcf, tbi -> [ meta - meta.subMap('normal_id', 'tumor_id','num_intervals') + [ variantcaller:'sage' ], vcf ] }
                           ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:22:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:28:93`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta, normal_cram, normal_crai, tumor_cram, tumor_crai, manta_vcf, manta_tbi, intervals_gz_tbi, num_intervals -> [ meta + [ num_intervals:0 ], normal_cram, normal_crai, tumor_cram, tumor_crai, manta_vcf, manta_tbi, [], [] ] }
                                                                                              ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:28:111`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta, normal_cram, normal_crai, tumor_cram, tumor_crai, manta_vcf, manta_tbi, intervals_gz_tbi, num_intervals -> [ meta + [ num_intervals:0 ], normal_cram, normal_crai, tumor_cram, tumor_crai, manta_vcf, manta_tbi, [], [] ] }
                                                                                                                ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:37:5`: Variable was declared but not used

  ```nextflow
      vcf_indels = STRELKA_SOMATIC.out.vcf_indels.branch{
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:39:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:40:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:44:5`: Variable was declared but not used

  ```nextflow
      vcf_snvs = STRELKA_SOMATIC.out.vcf_snvs.branch{
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:46:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:47:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/channel_baserecalibrator_create_csv/main.nf:8:9`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          tools
          ^^^^^
  ```

- Warning: `subworkflows/local/cram_merge_index_samtools/main.nf:17:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/cram_merge_index_samtools/main.nf:38:5`: Variable was declared but not used

  ```nextflow
      cram_crai = cram_all.join(INDEX_CRAM.out.index, failOnDuplicate: true, failOnMismatch: true)
      ^^^^^^^^^
  ```

- Warning: `subworkflows/local/cram_qc_mosdepth_samtools/main.nf:18:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/cram_qc_mosdepth_samtools/main.nf:19:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      reports = Channel.empty()
                ^^^^^^^
  ```

- Warning: `subworkflows/local/cram_qc_mosdepth_samtools/main.nf:29:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          cram.combine(intervals.map{ meta, bed -> [ bed?:[] ] }),
                                      ^^^^
  ```

- Warning: `subworkflows/local/fastq_align/main.nf:19:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/fastq_align/main.nf:20:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      reports = Channel.empty()
                ^^^^^^^
  ```

- Warning: `subworkflows/local/fastq_align/main.nf:29:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      bam = Channel.empty()
            ^^^^^^^
  ```

- Warning: `subworkflows/local/maf_filtering/main.nf:17:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions  = Channel.empty()
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/maf_filtering/main.nf:18:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      maf       = Channel.empty()
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/maf_rna_filtering/main.nf:11:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      fasta_fai
      ^^^^^^^^^
  ```

- Warning: `subworkflows/local/maf_rna_filtering/main.nf:15:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/maf_rna_filtering/main.nf:26:61`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              input_sample_type = input_sample.branch { meta, maf ->
                                                              ^^^
  ```

- Warning: `subworkflows/local/maf_rna_filtering/main.nf:35:43`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  maf_to_filter_realigned = Channel.empty()
                                            ^^^^^^^
  ```

- Warning: `subworkflows/local/maf_rna_filtering/main.nf:84:9`: Emit name should be omitted when there is only one emit

  ```nextflow
          versions            = versions // channel: [ versions.yml ]
          ^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:43:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:47:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          GUNZIP_FASTA(Channel.fromPath(params.fasta).collect().map{ fa -> [[id: fa.baseName[0] - ~/\.fa(sta)?$/], fa] })
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:71:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          bwa        = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:72:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          bwamem2    = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:73:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          hashtable  = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:122:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                      Channel.fromPath(params.gtf).map{ it -> [[id:it[0].baseName], it] }
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:127:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ch_gtf = Channel.fromPath(params.gtf).collect().map{gtf -> [[id:"gtf"], gtf]}
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:132:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                      Channel.fromPath(params.gff).map{ it -> [[id:it[0].baseName], it] }
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:137:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ch_gff = Channel.fromPath(params.gff).collect().map{gff -> [[id:"gff"], gff]}
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:156:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                      Channel.fromPath(params.star_index).map{ it -> [[id:it[0].baseName], it] }
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:161:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ch_star_index = Channel.fromPath(params.star_index).collect().map{star_index -> [[id:"star_index"], star_index]}
                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:174:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ch_splicesites  = Channel.fromPath(params.splicesites).collect().map{ it -> [ [ id:'null' ], it ]}
                                    ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:182:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ch_hisat2_index  = Channel.fromPath(params.hisat2_index).collect().map{it -> [ [ id:"hisat2_index" ], it ]}
                                     ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:197:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_star_index   = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:198:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gtf          = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:199:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_hisat2_index = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:200:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_splicesites  = Channel.value([])
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:222:61`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          dbsnp                 = TABIX_DBSNP.out.output.map{ meta, gz -> [gz] }.collect()
                                                              ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:223:60`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          dbsnp_tbi             = TABIX_DBSNP.out.index.map{ meta, tbi -> [tbi] }.collect()               // path: dbsnb.vcf.gz.tbi
                                                             ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:227:73`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          germline_resource     = TABIX_GERMLINE_RESOURCE.out.output.map{ meta, gz -> [gz] }.collect()
                                                                          ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:228:72`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          germline_resource_tbi = TABIX_GERMLINE_RESOURCE.out.index.map{ meta, tbi -> [tbi] }.collect()   // path: germline_resource.vcf.gz.tbi
                                                                         ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:229:66`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          known_snps            = TABIX_KNOWN_SNPS.out.output.map{ meta, gz -> [gz] }.collect()
                                                                   ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:230:65`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          known_snps_tbi        = TABIX_KNOWN_SNPS.out.index.map{ meta, tbi -> [tbi] }.collect()          // path: {known_indels*}.vcf.gz.tbi
                                                                  ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:231:68`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          known_indels          = TABIX_KNOWN_INDELS.out.output.map{ meta, gz -> [gz] }.collect()
                                                                     ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:232:67`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          known_indels_tbi      = TABIX_KNOWN_INDELS.out.index.map{ meta, tbi -> [tbi] }.collect()        // path: {known_indels*}.vcf.gz.tbi
                                                                    ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:233:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          pon                   = TABIX_PON.out.output.map{ meta, gz -> [gz] }.collect()
                                                            ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:234:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          pon_tbi               = TABIX_PON.out.index.map{ meta, tbi -> [tbi] }.collect()                 // path: pon.vcf.gz.tbi
                                                           ^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:25:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:29:50`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          intervals_bed                          = Channel.of([[], 0 ])
                                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:30:50`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          intervals_bed_gz_tbi                   = Channel.of([[[],[]], 0 ])
                                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:31:50`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          intervals_combined                     = Channel.of([[id:"no_intervals"], 0 ])
                                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:32:50`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          intervals_bed_gz_tbi_combined          = Channel.of([[], []])
                                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:33:50`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          intervals_bed_gz_tbi_and_num_intervals = Channel.of([[],[], 0 ])
                                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:41:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              CREATE_INTERVALS_BED(intervals_combined.map{ meta, path -> path }).bed
                                                           ^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:48:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              intervals_combined = Channel.fromPath(file(intervals)).map{it -> [ [ id:it.baseName ], it ] }
                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:79:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .flatten().collate(2).map{ duration, intervalFile -> intervalFile }.collect()
                                         ^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:86:38`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              intervals_bed.map{ file, num_intervals -> [ [ id:file.baseName], file, [], [] ] },
                                       ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:94:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map{ meta, bed, tbi -> [ bed, tbi ] }.toList()
                    ^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:114:18`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map{meta, gz, tbi -> [gz, tbi] }.collect()
                   ^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:123:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.value([]) :
          ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:124:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          intervals_combined.map{meta, bed -> bed }.collect()
                                 ^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:126:5`: Variable was declared but not used

  ```nextflow
      intervals_for_preprocessing = wes ?
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:128:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.value([ [ id:'null' ], [] ])
          ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:130:5`: Variable was declared but not used

  ```nextflow
      intervals_and_num_intervals   = intervals_bed.map{ interval, num_intervals ->
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_realignment/main.nf:24:9`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          dict        // channel: [mandatory] [ meta, dict ]
          ^^^^
  ```

- Warning: `subworkflows/local/prepare_realignment/main.nf:31:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          versions   = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_realignment/main.nf:32:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          bam_mapped = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_realignment/main.nf:40:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                          norealign: it[0].status == 1
                                                     ^^
  ```

- Warning: `subworkflows/local/prepare_realignment/main.nf:41:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                          realign:   it[0].status == 2 || it[0].status == 0
                                                     ^^
  ```

- Warning: `subworkflows/local/prepare_realignment/main.nf:41:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                          realign:   it[0].status == 2 || it[0].status == 0
                                                                          ^^
  ```

- Warning: `subworkflows/local/prepare_realignment/main.nf:46:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                          isconsensus: it[0].consensus == true
                                                       ^^
  ```

- Warning: `subworkflows/local/prepare_realignment/main.nf:47:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                          noconsensus: it[0].consensus == false
                                                       ^^
  ```

- Warning: `subworkflows/local/prepare_realignment/main.nf:64:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                          norealign: it[0].status == 1
                                                     ^^
  ```

- Warning: `subworkflows/local/prepare_realignment/main.nf:65:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                          realign:   it[0].status == 2 || it[0].status == 0
                                                     ^^
  ```

- Warning: `subworkflows/local/prepare_realignment/main.nf:65:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                          realign:   it[0].status == 2 || it[0].status == 0
                                                                          ^^
  ```

- Warning: `subworkflows/local/prepare_realignment/main.nf:68:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                          norealign: it[0].status == 1
                                                     ^^
  ```

- Warning: `subworkflows/local/prepare_realignment/main.nf:69:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                          realign:   it[0].status == 2 || it[0].status == 0
                                                     ^^
  ```

- Warning: `subworkflows/local/prepare_realignment/main.nf:69:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                          realign:   it[0].status == 2 || it[0].status == 0
                                                                          ^^
  ```

- Warning: `subworkflows/local/prepare_realignment/main.nf:146:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      bam_mapped = bam_mapped.map{meta, bam, index -> [meta - meta.subMap('single_end'), bam]}
                                             ^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:35:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:37:53`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      dbsnp              = dbsnp_input              ? Channel.fromPath(dbsnp_input).collect()                    : Channel.value([])
                                                      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:37:114`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      dbsnp              = dbsnp_input              ? Channel.fromPath(dbsnp_input).collect()                    : Channel.value([])
                                                                                                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:38:53`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      known_snps         = known_snps_input         ? Channel.fromPath(known_snps_input).collect()               : Channel.value([])
                                                      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:38:114`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      known_snps         = known_snps_input         ? Channel.fromPath(known_snps_input).collect()               : Channel.value([])
                                                                                                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:39:53`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      fasta              = fasta_input              ? Channel.fromPath(fasta_input).collect()                    : Channel.empty()
                                                      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:39:114`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      fasta              = fasta_input              ? Channel.fromPath(fasta_input).collect()                    : Channel.empty()
                                                                                                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:40:53`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      germline_resource  = germline_resource_input  ? Channel.fromPath(germline_resource_input).collect()        : Channel.value([]) //Mutec2 does not require a germline resource, so set to optional input
                                                      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:40:114`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      germline_resource  = germline_resource_input  ? Channel.fromPath(germline_resource_input).collect()        : Channel.value([]) //Mutec2 does not require a germline resource, so set to optional input
                                                                                                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:41:53`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      known_indels       = known_indels_input       ? Channel.fromPath(known_indels_input).collect()             : Channel.value([])
                                                      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:41:114`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      known_indels       = known_indels_input       ? Channel.fromPath(known_indels_input).collect()             : Channel.value([])
                                                                                                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:42:53`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      pon                = pon_input                ? Channel.fromPath(pon_input).collect()                      : Channel.value([]) //PON is optional for Mutect2 (but highly recommended)
                                                      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:42:114`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      pon                = pon_input                ? Channel.fromPath(pon_input).collect()                      : Channel.value([]) //PON is optional for Mutect2 (but highly recommended)
                                                                                                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:43:5`: Variable was declared but not used

  ```nextflow
      whitelist          = whitelist_input          ? Channel.fromPath(whitelist_input).collect()                : Channel.value([]) // whitelist optional for filtering
      ^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:43:53`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      whitelist          = whitelist_input          ? Channel.fromPath(whitelist_input).collect()                : Channel.value([]) // whitelist optional for filtering
                                                      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:43:114`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      whitelist          = whitelist_input          ? Channel.fromPath(whitelist_input).collect()                : Channel.value([]) // whitelist optional for filtering
                                                                                                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:57:5`: Variable was declared but not used

  ```nextflow
      bwa                    = fasta_input                   ? bwa_input                        ? Channel.fromPath(bwa_input).collect()                           : PREPARE_GENOME.out.bwa                   : []
      ^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:57:97`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      bwa                    = fasta_input                   ? bwa_input                        ? Channel.fromPath(bwa_input).collect()                           : PREPARE_GENOME.out.bwa                   : []
                                                                                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:58:5`: Variable was declared but not used

  ```nextflow
      bwamem2                = fasta_input                   ? bwamem2_input                    ? Channel.fromPath(bwamem2_input).collect()                       : PREPARE_GENOME.out.bwamem2               : []
      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:58:97`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      bwamem2                = fasta_input                   ? bwamem2_input                    ? Channel.fromPath(bwamem2_input).collect()                       : PREPARE_GENOME.out.bwamem2               : []
                                                                                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:59:5`: Variable was declared but not used

  ```nextflow
      dragmap                = fasta_input                   ? dragmap_input                    ? Channel.fromPath(dragmap_input).collect()                       : PREPARE_GENOME.out.hashtable             : []
      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:59:97`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      dragmap                = fasta_input                   ? dragmap_input                    ? Channel.fromPath(dragmap_input).collect()                       : PREPARE_GENOME.out.hashtable             : []
                                                                                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:60:5`: Variable was declared but not used

  ```nextflow
      hisat2_index           = fasta_input                   ? hisat2_index_input               ? Channel.fromPath(hisat2_index_input).map{ it -> [ [id:'ht_idx'], it ] }.collect()                          : PREPARE_GENOME.out.hisat2_index : []
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:60:97`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      hisat2_index           = fasta_input                   ? hisat2_index_input               ? Channel.fromPath(hisat2_index_input).map{ it -> [ [id:'ht_idx'], it ] }.collect()                          : PREPARE_GENOME.out.hisat2_index : []
                                                                                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:61:5`: Variable was declared but not used

  ```nextflow
      splicesites            = fasta_input                   ? splicesites_input                ? Channel.fromPath(splicesites_input).collect()                   : PREPARE_GENOME.out.splicesites           : []
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:61:97`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      splicesites            = fasta_input                   ? splicesites_input                ? Channel.fromPath(splicesites_input).collect()                   : PREPARE_GENOME.out.splicesites           : []
                                                                                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:62:5`: Variable was declared but not used

  ```nextflow
      dict                   = dict_input                    ? Channel.fromPath(dict_input).map{ it -> [ [id:'dict'], it ] }.first()                               : PREPARE_GENOME.out.dict
      ^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:62:62`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      dict                   = dict_input                    ? Channel.fromPath(dict_input).map{ it -> [ [id:'dict'], it ] }.first()                               : PREPARE_GENOME.out.dict
                                                               ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:63:97`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      fasta_fai              = fasta_input                   ? fasta_fai_input                  ? Channel.fromPath(fasta_fai_input).collect()                     : PREPARE_GENOME.out.fasta_fai             : []
                                                                                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:66:97`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      dbsnp                  = dbsnp_input                   ? dbsnp_tbi_input                  ? Channel.fromPath(dbsnp_input).collect()                         : PREPARE_GENOME.out.dbsnp                  : Channel.value([])
                                                                                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:66:207`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      dbsnp                  = dbsnp_input                   ? dbsnp_tbi_input                  ? Channel.fromPath(dbsnp_input).collect()                         : PREPARE_GENOME.out.dbsnp                  : Channel.value([])
                                                                                                                                                                                                                ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:67:97`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      germline_resource      = germline_resource_input       ? germline_resource_tbi_input      ? Channel.fromPath(germline_resource_input).collect()             : PREPARE_GENOME.out.germline_resource      : []
                                                                                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:68:97`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      known_indels           = known_indels_input            ? known_indels_tbi_input           ? Channel.fromPath(known_indels_input).collect()                  : PREPARE_GENOME.out.known_indels           : Channel.value([])
                                                                                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:68:207`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      known_indels           = known_indels_input            ? known_indels_tbi_input           ? Channel.fromPath(known_indels_input).collect()                  : PREPARE_GENOME.out.known_indels           : Channel.value([])
                                                                                                                                                                                                                ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:69:97`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      known_snps             = known_snps_input              ? known_snps_tbi_input             ? Channel.fromPath(known_snps_input).collect()                    : PREPARE_GENOME.out.known_snps             : Channel.value([])
                                                                                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:69:207`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      known_snps             = known_snps_input              ? known_snps_tbi_input             ? Channel.fromPath(known_snps_input).collect()                    : PREPARE_GENOME.out.known_snps             : Channel.value([])
                                                                                                                                                                                                                ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:70:97`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      pon                    = pon_input                     ? pon_tbi_input                    ? Channel.fromPath(pon_input).collect()                           : PREPARE_GENOME.out.pon                    : []
                                                                                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:71:97`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      dbsnp_tbi              = dbsnp_input                   ? dbsnp_tbi_input                  ? Channel.fromPath(dbsnp_tbi_input).collect()                     : PREPARE_GENOME.out.dbsnp_tbi             : Channel.value([])
                                                                                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:71:206`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      dbsnp_tbi              = dbsnp_input                   ? dbsnp_tbi_input                  ? Channel.fromPath(dbsnp_tbi_input).collect()                     : PREPARE_GENOME.out.dbsnp_tbi             : Channel.value([])
                                                                                                                                                                                                               ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:72:5`: Variable was declared but not used

  ```nextflow
      germline_resource_tbi  = germline_resource_input       ? germline_resource_tbi_input      ? Channel.fromPath(germline_resource_tbi_input).collect()         : PREPARE_GENOME.out.germline_resource_tbi : []
      ^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:72:97`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      germline_resource_tbi  = germline_resource_input       ? germline_resource_tbi_input      ? Channel.fromPath(germline_resource_tbi_input).collect()         : PREPARE_GENOME.out.germline_resource_tbi : []
                                                                                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:73:97`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      known_indels_tbi       = known_indels_input            ? known_indels_tbi_input           ? Channel.fromPath(known_indels_tbi_input).collect()              : PREPARE_GENOME.out.known_indels_tbi      : Channel.value([])
                                                                                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:73:206`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      known_indels_tbi       = known_indels_input            ? known_indels_tbi_input           ? Channel.fromPath(known_indels_tbi_input).collect()              : PREPARE_GENOME.out.known_indels_tbi      : Channel.value([])
                                                                                                                                                                                                               ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:74:97`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      known_snps_tbi         = known_snps_input              ? known_snps_tbi_input             ? Channel.fromPath(known_snps_tbi_input).collect()                : PREPARE_GENOME.out.known_snps_tbi        : Channel.value([])
                                                                                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:74:206`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      known_snps_tbi         = known_snps_input              ? known_snps_tbi_input             ? Channel.fromPath(known_snps_tbi_input).collect()                : PREPARE_GENOME.out.known_snps_tbi        : Channel.value([])
                                                                                                                                                                                                               ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:75:5`: Variable was declared but not used

  ```nextflow
      pon_tbi                = pon_input                     ? pon_tbi_input                    ? Channel.fromPath(pon_tbi_input).collect()                       : PREPARE_GENOME.out.pon_tbi               : []
      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:75:97`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      pon_tbi                = pon_input                     ? pon_tbi_input                    ? Channel.fromPath(pon_tbi_input).collect()                       : PREPARE_GENOME.out.pon_tbi               : []
                                                                                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:78:5`: Variable was declared but not used

  ```nextflow
      known_sites_indels     = dbsnp.concat(known_indels).collect()
      ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:79:5`: Variable was declared but not used

  ```nextflow
      known_sites_indels_tbi = dbsnp_tbi.concat(known_indels_tbi).collect()
      ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:81:5`: Variable was declared but not used

  ```nextflow
      known_sites_snps       = dbsnp.concat(known_snps).collect()
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_and_intervals/main.nf:82:5`: Variable was declared but not used

  ```nextflow
      known_sites_snps_tbi   = dbsnp_tbi.concat(known_snps_tbi).collect()
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/samplesheet_to_channel/main.nf:25:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { patient_sample, num_lanes, ch_items ->
                 ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/samplesheet_to_channel/main.nf:216:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      input_sample
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/samplesheet_to_channel/main.nf:232:68`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          InputStream gzipStream = new java.util.zip.GZIPInputStream(it)
                                                                     ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_rnadnavar_pipeline/main.nf:40:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_rnadnavar_pipeline/main.nf:107:9`: Variable was declared but not used

  ```nextflow
      def checkPathParamList = [
          ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_rnadnavar_pipeline/main.nf:149:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ? Channel.empty()
            ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_rnadnavar_pipeline/main.nf:150:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.fromList(parsed_samplesheet)
            ^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_annotate/main.nf:18:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      reports  = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_annotate/main.nf:19:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_ann  = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_annotate/main.nf:20:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tab_ann  = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_annotate/main.nf:21:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      json_ann = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_annotate/main.nf:28:63`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              vep_cache_version  = params.vep_cache_version  ?: Channel.empty()
                                                                ^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_annotate/main.nf:29:63`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              vep_genome         = params.vep_genome         ?: Channel.empty()
                                                                ^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_annotate/main.nf:30:63`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              vep_species        = params.vep_species        ?: Channel.empty()
                                                                ^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:24:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions                = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:26:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      maf_from_consensus_dna  = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:27:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      mafs_from_varcal_dna    = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:28:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      consensus_maf           = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:41:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                  vcf: it[0].data_type == "vcf"
                                       ^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:42:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                  maf: it[0].data_type == "maf"
                                       ^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:48:69`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              tools_list = params.tools.split(',').toList().findAll { it in ['sage', 'strelka', 'mutect2'] }.unique()
                                                                      ^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:54:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch { meta, vcf_file ->
                        ^^^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:69:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              Channel.value([]) // empty vep - we already call it independently
              ^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:90:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      [meta, paired.collect { it[1] }, paired.collect { it[0] }]
                                              ^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:90:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      [meta, paired.collect { it[1] }, paired.collect { it[0] }]
                                                                        ^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:103:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                  dna: it[0].status <= 1
                                       ^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:104:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                  rna: it[0].status == 2
                                       ^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:108:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                  dna: it[0].status <= 1
                                       ^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:109:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                  rna: it[0].status == 2
                                       ^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:170:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                                      [meta, paired.collect { it[1] }, paired.collect { it[0] }]
                                                                              ^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:170:103`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                                      [meta, paired.collect { it[1] }, paired.collect { it[0] }]
                                                                                                        ^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:183:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                                  [meta, paired.collect { it[1] }, paired.collect { it[0] }]
                                                                          ^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:183:99`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                                  [meta, paired.collect { it[1] }, paired.collect { it[0] }]
                                                                                                    ^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:186:13`: Variable was declared but not used

  ```nextflow
              mafs_to_rescue = mafs_dna_crossed_with_rna_rescue.mix(mafs_rna_crossed_with_dna_rescue)
              ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:190:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                  dna: it[0].status <= 1
                                       ^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:191:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                  rna: it[0].status == 2
                                       ^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:195:13`: Variable was declared but not used

  ```nextflow
              run_rescue_out = RUN_CONSENSUS_RESCUE.out.maf.branch{
              ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:196:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  intervals:    it[0].num_intervals > 1
                                ^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:197:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  no_intervals: it[0].num_intervals <= 1
                                ^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:222:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                  vcf: it[0].data_type == "vcf"
                                       ^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:223:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                  maf: it[0].data_type == "maf"
                                       ^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:227:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .branch { meta, vcf_file ->
                            ^^^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:242:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  Channel.value([]) // empty vep - we already call it independently
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_normalize/main.nf:22:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      version          = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_normalize/main.nf:32:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          vcf_decomposed  = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_qc_bcftools_vcftools/main.nf:13:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
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

- Warning: `workflows/rnadnavar/main.nf:57:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `workflows/rnadnavar/main.nf:58:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      multiqc_report = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `workflows/rnadnavar/main.nf:59:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      reports = Channel.empty()
                ^^^^^^^
  ```

- Warning: `workflows/rnadnavar/main.nf:61:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `workflows/rnadnavar/main.nf:65:48`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      mutect2_alleles = params.mutect2_alleles ? Channel.value(file(params.mutect2_alleles, checkIfExists: true)) : Channel.value([])
                                                 ^^^^^^^
  ```

- Warning: `workflows/rnadnavar/main.nf:65:115`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      mutect2_alleles = params.mutect2_alleles ? Channel.value(file(params.mutect2_alleles, checkIfExists: true)) : Channel.value([])
                                                                                                                    ^^^^^^^
  ```

- Warning: `workflows/rnadnavar/main.nf:66:56`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      mutect2_alleles_tbi = params.mutect2_alleles_tbi ? Channel.value(file(params.mutect2_alleles_tbi, checkIfExists: true)) : Channel.value([])
                                                         ^^^^^^^
  ```

- Warning: `workflows/rnadnavar/main.nf:66:127`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      mutect2_alleles_tbi = params.mutect2_alleles_tbi ? Channel.value(file(params.mutect2_alleles_tbi, checkIfExists: true)) : Channel.value([])
                                                                                                                                ^^^^^^^
  ```

- Warning: `workflows/rnadnavar/main.nf:79:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ensemblvep_info = Channel.of([[id: "${params.vep_cache_version}_${params.vep_genome}"], params.vep_genome, params.vep_species, params.vep_cache_version])
                            ^^^^^^^
  ```

- Warning: `workflows/rnadnavar/main.nf:86:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          UNZIP_VEP_CACHE(Channel.fromPath(params.vep_cache).collect().map { it -> [[id: it[0].baseName], it] })
                          ^^^^^^^
  ```

- Warning: `workflows/rnadnavar/main.nf:151:5`: Variable was declared but not used

  ```nextflow
      known_sites_snps = PREPARE_REFERENCE_AND_INTERVALS.out.known_sites_snps
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/rnadnavar/main.nf:152:5`: Variable was declared but not used

  ```nextflow
      known_sites_snps_tbi = PREPARE_REFERENCE_AND_INTERVALS.out.known_sites_snps_tbi
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/rnadnavar/main.nf:238:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              Channel.empty(),
              ^^^^^^^
  ```

- Warning: `workflows/rnadnavar/main.nf:240:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              Channel.empty(),
              ^^^^^^^
  ```

- Warning: `workflows/rnadnavar/main.nf:272:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          realigned_filtered_maf = Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `workflows/rnadnavar/main.nf:278:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              dna: it[0].status < 2
                   ^^
  ```

- Warning: `workflows/rnadnavar/main.nf:279:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              rna: it[0].status >= 2
                   ^^
  ```

- Warning: `workflows/rnadnavar/main.nf:282:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              dna: it[0].status < 2
                   ^^
  ```

- Warning: `workflows/rnadnavar/main.nf:283:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              rna: it[0].status >= 2
                   ^^
  ```

- Warning: `workflows/rnadnavar/main.nf:293:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      version_yaml = Channel.empty()
                     ^^^^^^^
  ```

- Warning: `workflows/rnadnavar/main.nf:323:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_workflow_summary = Channel.value(paramsSummaryMultiqc(summary_params))
                                ^^^^^^^
  ```

- Warning: `workflows/rnadnavar/main.nf:325:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_methods_description = Channel.value(methodsDescriptionText(ch_multiqc_custom_methods_description))
                                   ^^^^^^^
  ```

- Warning: `workflows/rnadnavar/main.nf:370:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def InputStream gzipStream = new java.util.zip.GZIPInputStream(it)
                                                                         ^^
  ```
