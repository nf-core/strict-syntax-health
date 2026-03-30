# Nextflow lint results

- Generated: 2026-03-30T00:24:57.384721308Z
- Nextflow version: 26.03.1-edge
- Summary: 71 warnings

## :warning: Warnings

- Warning: `conf/modules.config:348:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { (meta.single_end || params.save_align_intermeds) ? "${it}" : null }
                                                                              ^^
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

- Warning: `subworkflows/local/bam_peaks_call_qc_annotate_macs3_homer/main.nf:46:13`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, peaks ->
              ^^^^
  ```

- Warning: `subworkflows/local/bam_peaks_call_qc_annotate_macs3_homer/main.nf:55:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, ip_bam, control_bam, peaks ->
                            ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_peaks_call_qc_annotate_macs3_homer/main.nf:71:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, ip_bam, peaks, frip ->
                    ^^^^^^
  ```

- Warning: `subworkflows/local/bam_peaks_call_qc_annotate_macs3_homer/main.nf:108:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_macs3_peaks.collect{it[1]},
                                         ^^
  ```

- Warning: `subworkflows/local/bam_peaks_call_qc_annotate_macs3_homer/main.nf:118:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  HOMER_ANNOTATEPEAKS.out.txt.collect{it[1]},
                                                      ^^
  ```

- Warning: `subworkflows/local/bed_consensus_quantify_qc_bedtools_featurecounts_deseq2/main.nf:26:5`: Variable was declared but not used

  ```nextflow
      ch_versions = channel.empty()
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bed_consensus_quantify_qc_bedtools_featurecounts_deseq2/main.nf:40:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      groups.groupBy().collectEntries { [(it.key) : it.value.size()] },
                                                          ^^
  ```

- Warning: `subworkflows/local/bed_consensus_quantify_qc_bedtools_featurecounts_deseq2/main.nf:40:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      groups.groupBy().collectEntries { [(it.key) : it.value.size()] },
                                                                    ^^
  ```

- Warning: `subworkflows/local/bed_consensus_quantify_qc_bedtools_featurecounts_deseq2/main.nf:49:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  meta_new.replicates_exist = groups.max { it.value }.value > 1
                                                           ^^
  ```

- Warning: `subworkflows/local/input_check/main.nf:16:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { create_fastq_channel(it, seq_center) }
                                      ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:43:5`: Variable was declared but not used

  ```nextflow
      ch_versions = channel.empty()
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:50:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta    = GUNZIP_FASTA([[:], fasta]).gunzip.map { it[1] }
                                                                ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:62:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gtf      = GUNZIP_GTF([[:], gtf]).gunzip.map { it[1] }
                                                                ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:68:90`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gff      = GUNZIP_GFF([[:], file(gff, checkIfExists: true)]).gunzip.map { it[1] }
                                                                                           ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:70:81`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gff = channel.value(file(gff, checkIfExists: true)).map { [ [:], it ] }
                                                                                  ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:73:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_gtf      = GFFREAD(ch_gff, []).gtf.map { it[1] }
                                                      ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:82:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_blacklist = GUNZIP_BLACKLIST([[:], blacklist]).gunzip.map { it[1] }
                                                                             ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:107:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gene_bed = GUNZIP_GENE_BED([[:], gene_bed]).gunzip.map { it[1] }
                                                                          ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:146:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_bwa_index = BWA_INDEX(ch_fasta.map { [[:], it] }).index
                                                            ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:162:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_bowtie2_index = BOWTIE2_BUILD(ch_fasta.map { [[:], it] }).index
                                                                    ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:178:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_chromap_index = CHROMAP_INDEX(ch_fasta.map { [[:], it] }).index
                                                                    ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:189:81`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_star_index = UNTAR_STAR_INDEX([[:], star_index]).untar.map { it[1] }
                                                                                  ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_chipseq_pipeline/main.nf:31:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_chipseq_pipeline/main.nf:122:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      hook_url        //  string: hook URL for notifications
      ^^^^^^^^
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

- Warning: `workflows/chipseq.nf:437:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_macs_gsize = KHMER_UNIQUEKMERS.out.kmers.map { meta, file ->
                                                            ^^^^
  ```

- Warning: `workflows/chipseq.nf:444:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, bams, bais ->
                          ^^^^
  ```

- Warning: `workflows/chipseq.nf:477:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, ip_bam, control_bam ->
                                ^^^^^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:514:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              BAM_BEDGRAPH_BIGWIG_BEDTOOLS_UCSC.out.bigwig.collect{it[1]}.ifEmpty([]),
                                                                   ^^
  ```

- Warning: `workflows/chipseq.nf:515:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              BAM_PEAKS_CALL_QC_ANNOTATE_MACS3_HOMER.out.peaks.collect{it[1]}.ifEmpty([]),
                                                                       ^^
  ```

- Warning: `workflows/chipseq.nf:516:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_macs3_consensus_bed_lib.collect{it[1]}.ifEmpty([]),
                                                 ^^
  ```

- Warning: `workflows/chipseq.nf:517:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_macs3_consensus_txt_lib.collect{it[1]}.ifEmpty([])
                                                 ^^
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
