# Nextflow lint results

- Generated: 2026-03-20T00:23:50.691512356Z
- Nextflow version: 26.03.0-edge
- Summary: 129 warnings

## :warning: Warnings

- Warning: `conf/modules.config:355:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { (meta.single_end || params.save_align_intermeds) ? "${it}" : null }
                                                                              ^^
  ```

- Warning: `main.nf:52:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `main.nf:73:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_samplesheet = Channel.value(file(params.input, checkIfExists: true))
                       ^^^^^^^
  ```

- Warning: `modules/local/macs3_consensus/main.nf:39:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      sort -T '.' -k1,1 -k2,2n ${peaks.collect{it.toString()}.sort().join(' ')} \\
                                               ^^
  ```

- Warning: `modules/local/macs3_consensus/main.nf:44:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ${peaks.collect{it.toString()}.sort().join(',').replaceAll("_peaks.${peak_type}","")} \\
                          ^^
  ```

- Warning: `subworkflows/local/bam_peaks_call_qc_annotate_macs3_homer/main.nf:44:13`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, peaks ->
              ^^^^
  ```

- Warning: `subworkflows/local/bam_peaks_call_qc_annotate_macs3_homer/main.nf:53:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, ip_bam, control_bam, peaks ->
                            ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_peaks_call_qc_annotate_macs3_homer/main.nf:69:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, ip_bam, peaks, frip ->
                    ^^^^^^
  ```

- Warning: `subworkflows/local/bam_peaks_call_qc_annotate_macs3_homer/main.nf:83:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_homer_annotatepeaks          = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_peaks_call_qc_annotate_macs3_homer/main.nf:84:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_plot_macs3_qc_txt            = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_peaks_call_qc_annotate_macs3_homer/main.nf:85:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_plot_macs3_qc_pdf            = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_peaks_call_qc_annotate_macs3_homer/main.nf:86:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_plot_homer_annotatepeaks_txt = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_peaks_call_qc_annotate_macs3_homer/main.nf:87:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_plot_homer_annotatepeaks_pdf = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_peaks_call_qc_annotate_macs3_homer/main.nf:88:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_plot_homer_annotatepeaks_tsv = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_peaks_call_qc_annotate_macs3_homer/main.nf:105:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_macs3_peaks.collect{it[1]},
                                         ^^
  ```

- Warning: `subworkflows/local/bam_peaks_call_qc_annotate_macs3_homer/main.nf:115:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  HOMER_ANNOTATEPEAKS.out.txt.collect{it[1]},
                                                      ^^
  ```

- Warning: `subworkflows/local/bed_consensus_quantify_qc_bedtools_featurecounts_deseq2/main.nf:39:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      groups.groupBy().collectEntries { [(it.key) : it.value.size()] },
                                                          ^^
  ```

- Warning: `subworkflows/local/bed_consensus_quantify_qc_bedtools_featurecounts_deseq2/main.nf:39:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      groups.groupBy().collectEntries { [(it.key) : it.value.size()] },
                                                                    ^^
  ```

- Warning: `subworkflows/local/bed_consensus_quantify_qc_bedtools_featurecounts_deseq2/main.nf:48:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  meta_new.replicates_exist = groups.max { it.value }.value > 1
                                                           ^^
  ```

- Warning: `subworkflows/local/bed_consensus_quantify_qc_bedtools_featurecounts_deseq2/main.nf:89:13`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              antibody, meta, saf, bams, meta_single_end ->
              ^^^^^^^^
  ```

- Warning: `subworkflows/local/bed_consensus_quantify_qc_bedtools_featurecounts_deseq2/main.nf:104:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_deseq2_qc_pdf           = Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/bed_consensus_quantify_qc_bedtools_featurecounts_deseq2/main.nf:105:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_deseq2_qc_rdata         = Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/bed_consensus_quantify_qc_bedtools_featurecounts_deseq2/main.nf:106:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_deseq2_qc_rds           = Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/bed_consensus_quantify_qc_bedtools_featurecounts_deseq2/main.nf:107:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_deseq2_qc_pca_txt       = Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/bed_consensus_quantify_qc_bedtools_featurecounts_deseq2/main.nf:108:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_deseq2_qc_pca_multiqc   = Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/bed_consensus_quantify_qc_bedtools_featurecounts_deseq2/main.nf:109:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_deseq2_qc_dists_txt     = Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/bed_consensus_quantify_qc_bedtools_featurecounts_deseq2/main.nf:110:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_deseq2_qc_dists_multiqc = Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/bed_consensus_quantify_qc_bedtools_featurecounts_deseq2/main.nf:111:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_deseq2_qc_log           = Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/bed_consensus_quantify_qc_bedtools_featurecounts_deseq2/main.nf:112:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_deseq2_qc_size_factors  = Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/input_check/main.nf:16:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { create_fastq_channel(it, seq_center) }
                                      ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:50:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_fasta = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:52:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta    = GUNZIP_FASTA([[:], fasta]).gunzip.map { it[1] }
                                                                ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:55:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_fasta = Channel.value(file(fasta, checkIfExists: true))
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:63:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gtf      = GUNZIP_GTF([[:], gtf]).gunzip.map { it[1] }
                                                                ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:65:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_gtf = Channel.value(file(gtf, checkIfExists: true))
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:69:90`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gff      = GUNZIP_GFF([[:], file(gff, checkIfExists: true)]).gunzip.map { it[1] }
                                                                                           ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:71:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_gff = Channel.value(file(gff, checkIfExists: true)).map { [ [:], it ] }
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:71:81`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gff = Channel.value(file(gff, checkIfExists: true)).map { [ [:], it ] }
                                                                                  ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:74:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_gtf      = GFFREAD(ch_gff, []).gtf.map { it[1] }
                                                      ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:80:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_blacklist = Channel.empty()
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:83:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_blacklist = GUNZIP_BLACKLIST([[:], blacklist]).gunzip.map { it[1] }
                                                                             ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:85:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_blacklist = Channel.value(file(blacklist))
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:108:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gene_bed = GUNZIP_GENE_BED([[:], gene_bed]).gunzip.map { it[1] }
                                                                          ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:110:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_gene_bed = Channel.value(file(gene_bed))
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:127:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_genome_filtered_bed = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:138:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_bwa_index = Channel.empty()
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:147:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_bwa_index = BWA_INDEX(ch_fasta.map { [[:], it] }).index
                                                            ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:154:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_bowtie2_index = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:163:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_bowtie2_index = BOWTIE2_BUILD(ch_fasta.map { [[:], it] }).index
                                                                    ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:170:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_chromap_index = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:179:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_chromap_index = CHROMAP_INDEX(ch_fasta.map { [[:], it] }).index
                                                                    ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:186:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_star_index = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:190:81`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_star_index = UNTAR_STAR_INDEX([[:], star_index]).untar.map { it[1] }
                                                                                  ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:192:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ch_star_index = Channel.value(file(star_index))
                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_chipseq_pipeline/main.nf:31:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_chipseq_pipeline/main.nf:102:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_samplesheet = Channel.fromList(samplesheetToList(input, "assets/schema_input.json"))
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_chipseq_pipeline/main.nf:122:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      hook_url        //  string: hook URL for notifications
      ^^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:94:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_deseq2_pca_header        = Channel.value(file("$projectDir/assets/multiqc/deseq2_pca_header.txt", checkIfExists: true))
                                    ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:95:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_deseq2_clustering_header = Channel.value(file("$projectDir/assets/multiqc/deseq2_clustering_header.txt", checkIfExists: true))
                                    ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:153:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_genome_bam        = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:154:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_genome_bam_index  = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:155:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_samtools_stats    = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:156:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_samtools_flagstat = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:157:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_samtools_idxstats = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:165:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      [ [:], it ]
                             ^^
  ```

- Warning: `workflows/chipseq.nf:186:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      [ [:], it ]
                             ^^
  ```

- Warning: `workflows/chipseq.nf:205:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      [ [:], it ]
                             ^^
  ```

- Warning: `workflows/chipseq.nf:228:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          [ [:], it ]
                                 ^^
  ```

- Warning: `workflows/chipseq.nf:234:9`: Variable was declared but not used

  ```nextflow
          ch_transcriptome_bam = ALIGN_STAR.out.bam_transcript
          ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:238:9`: Variable was declared but not used

  ```nextflow
          ch_star_multiqc      = ALIGN_STAR.out.log_final
          ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:270:24`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  [ [:], it ]
                         ^^
  ```

- Warning: `workflows/chipseq.nf:274:24`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  [ [:], it ]
                         ^^
  ```

- Warning: `workflows/chipseq.nf:286:24`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  [ [:], it ]
                         ^^
  ```

- Warning: `workflows/chipseq.nf:295:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_preseq_multiqc = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:306:47`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_picardcollectmultiplemetrics_multiqc = Channel.empty()
                                                ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:313:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      [ it[0], it[1], [] ]
                        ^^
  ```

- Warning: `workflows/chipseq.nf:313:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      [ it[0], it[1], [] ]
                               ^^
  ```

- Warning: `workflows/chipseq.nf:317:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      [ [:], it ]
                             ^^
  ```

- Warning: `workflows/chipseq.nf:321:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      [ [:], it ]
                             ^^
  ```

- Warning: `workflows/chipseq.nf:330:59`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_phantompeakqualtools_spp_multiqc                 = Channel.empty()
                                                            ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:331:59`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_phantompeakqualtools_nsc_multiqc         = Channel.empty()
                                                            ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:332:59`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_phantompeakqualtools_rsc_multiqc         = Channel.empty()
                                                            ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:333:59`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_phantompeakqualtools_correlation_multiqc = Channel.empty()
                                                            ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:363:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_deeptoolsplotprofile_multiqc = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:417:43`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_deeptoolsplotfingerprint_multiqc = Channel.empty()
                                            ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:428:41`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_macs_gsize                     = Channel.empty()
                                          ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:429:41`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_subreadfeaturecounts_multiqc   = Channel.empty()
                                          ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:437:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_macs_gsize = KHMER_UNIQUEKMERS.out.kmers.map { meta, file ->
                                                            ^^^^
  ```

- Warning: `workflows/chipseq.nf:445:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, bams, bais ->
                          ^^^^
  ```

- Warning: `workflows/chipseq.nf:470:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_macs3_consensus_bed_lib   = Channel.empty()
                                     ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:471:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_macs3_consensus_txt_lib   = Channel.empty()
                                     ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:472:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_deseq2_pca_multiqc        = Channel.empty()
                                     ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:473:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_deseq2_clustering_multiqc = Channel.empty()
                                     ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:478:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, ip_bam, control_bam ->
                                ^^^^^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:515:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              BAM_BEDGRAPH_BIGWIG_BEDTOOLS_UCSC.out.bigwig.collect{it[1]}.ifEmpty([]),
                                                                   ^^
  ```

- Warning: `workflows/chipseq.nf:516:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              BAM_PEAKS_CALL_QC_ANNOTATE_MACS3_HOMER.out.peaks.collect{it[1]}.ifEmpty([]),
                                                                       ^^
  ```

- Warning: `workflows/chipseq.nf:517:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_macs3_consensus_bed_lib.collect{it[1]}.ifEmpty([]),
                                                 ^^
  ```

- Warning: `workflows/chipseq.nf:518:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_macs3_consensus_txt_lib.collect{it[1]}.ifEmpty([])
                                                 ^^
  ```

- Warning: `workflows/chipseq.nf:537:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_report = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:540:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_multiqc_config        = Channel.fromPath("$projectDir/assets/multiqc_config.yml", checkIfExists: true)
                                     ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:541:60`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_multiqc_custom_config = params.multiqc_config ? Channel.fromPath( params.multiqc_config ): Channel.empty()
                                                             ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:541:103`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_multiqc_custom_config = params.multiqc_config ? Channel.fromPath( params.multiqc_config ): Channel.empty()
                                                                                                        ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:542:60`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_multiqc_logo          = params.multiqc_logo   ? Channel.fromPath( params.multiqc_logo )  : Channel.empty()
                                                             ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:542:103`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_multiqc_logo          = params.multiqc_logo   ? Channel.fromPath( params.multiqc_logo )  : Channel.empty()
                                                                                                        ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:544:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_workflow_summary      = Channel.value(paramsSummaryMultiqc(summary_params))
                                     ^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:554:69`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              FASTQ_FASTQC_UMITOOLS_TRIMGALORE.out.fastqc_zip.collect{it[1]}.ifEmpty([]),
                                                                      ^^
  ```

- Warning: `workflows/chipseq.nf:555:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              FASTQ_FASTQC_UMITOOLS_TRIMGALORE.out.trim_zip.collect{it[1]}.ifEmpty([]),
                                                                    ^^
  ```

- Warning: `workflows/chipseq.nf:556:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              FASTQ_FASTQC_UMITOOLS_TRIMGALORE.out.trim_log.collect{it[1]}.ifEmpty([]),
                                                                    ^^
  ```

- Warning: `workflows/chipseq.nf:558:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_samtools_stats.collect{it[1]}.ifEmpty([]),
                                        ^^
  ```

- Warning: `workflows/chipseq.nf:559:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_samtools_flagstat.collect{it[1]}.ifEmpty([]),
                                           ^^
  ```

- Warning: `workflows/chipseq.nf:560:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_samtools_idxstats.collect{it[1]}.ifEmpty([]),
                                           ^^
  ```

- Warning: `workflows/chipseq.nf:562:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              BAM_MARKDUPLICATES_PICARD.out.stats.collect{it[1]}.ifEmpty([]),
                                                          ^^
  ```

- Warning: `workflows/chipseq.nf:563:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              BAM_MARKDUPLICATES_PICARD.out.flagstat.collect{it[1]}.ifEmpty([]),
                                                             ^^
  ```

- Warning: `workflows/chipseq.nf:564:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              BAM_MARKDUPLICATES_PICARD.out.idxstats.collect{it[1]}.ifEmpty([]),
                                                             ^^
  ```

- Warning: `workflows/chipseq.nf:565:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              BAM_MARKDUPLICATES_PICARD.out.metrics.collect{it[1]}.ifEmpty([]),
                                                            ^^
  ```

- Warning: `workflows/chipseq.nf:567:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              BAM_FILTER_BAMTOOLS.out.stats.collect{it[1]}.ifEmpty([]),
                                                    ^^
  ```

- Warning: `workflows/chipseq.nf:568:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              BAM_FILTER_BAMTOOLS.out.flagstat.collect{it[1]}.ifEmpty([]),
                                                       ^^
  ```

- Warning: `workflows/chipseq.nf:569:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              BAM_FILTER_BAMTOOLS.out.idxstats.collect{it[1]}.ifEmpty([]),
                                                       ^^
  ```

- Warning: `workflows/chipseq.nf:570:61`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_picardcollectmultiplemetrics_multiqc.collect{it[1]}.ifEmpty([]),
                                                              ^^
  ```

- Warning: `workflows/chipseq.nf:572:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_preseq_multiqc.collect{it[1]}.ifEmpty([]),
                                        ^^
  ```

- Warning: `workflows/chipseq.nf:574:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_deeptoolsplotprofile_multiqc.collect{it[1]}.ifEmpty([]),
                                                      ^^
  ```

- Warning: `workflows/chipseq.nf:575:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_deeptoolsplotfingerprint_multiqc.collect{it[1]}.ifEmpty([]),
                                                          ^^
  ```

- Warning: `workflows/chipseq.nf:577:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_phantompeakqualtools_spp_multiqc.collect{it[1]}.ifEmpty([]),
                                                          ^^
  ```

- Warning: `workflows/chipseq.nf:578:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_phantompeakqualtools_nsc_multiqc.collect{it[1]}.ifEmpty([]),
                                                                  ^^
  ```

- Warning: `workflows/chipseq.nf:579:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_phantompeakqualtools_rsc_multiqc.collect{it[1]}.ifEmpty([]),
                                                                  ^^
  ```

- Warning: `workflows/chipseq.nf:580:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_phantompeakqualtools_correlation_multiqc.collect{it[1]}.ifEmpty([]),
                                                                          ^^
  ```

- Warning: `workflows/chipseq.nf:582:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              BAM_PEAKS_CALL_QC_ANNOTATE_MACS3_HOMER.out.frip_multiqc.collect{it[1]}.ifEmpty([]),
                                                                              ^^
  ```

- Warning: `workflows/chipseq.nf:583:83`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              BAM_PEAKS_CALL_QC_ANNOTATE_MACS3_HOMER.out.peak_count_multiqc.collect{it[1]}.ifEmpty([]),
                                                                                    ^^
  ```

- Warning: `workflows/chipseq.nf:585:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_subreadfeaturecounts_multiqc.collect{it[1]}.ifEmpty([]),
                                                      ^^
  ```
