# Nextflow lint results

- Generated: 2026-07-23T00:30:09.893038452Z
- Nextflow version: 26.07.0-edge
- Summary: 57 warnings

## :warning: Warnings

- Warning: `conf/modules.config:358:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

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

- Warning: `subworkflows/local/bed_consensus_quantify_qc_bedtools_featurecounts_deseq2/main.nf:38:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      groups.groupBy().collectEntries { [(it.key) : it.value.size()] },
                                                          ^^
  ```

- Warning: `subworkflows/local/bed_consensus_quantify_qc_bedtools_featurecounts_deseq2/main.nf:38:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      groups.groupBy().collectEntries { [(it.key) : it.value.size()] },
                                                                    ^^
  ```

- Warning: `subworkflows/local/bed_consensus_quantify_qc_bedtools_featurecounts_deseq2/main.nf:47:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  meta_new.replicates_exist = groups.max { it.value }.value > 1
                                                           ^^
  ```

- Warning: `subworkflows/local/input_check/main.nf:16:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { create_fastq_channel(it, seq_center) }
                                      ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:46:5`: Variable was declared but not used

  ```nextflow
      ch_versions = channel.empty()
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:53:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta = GUNZIP_FASTA([[:], fasta]).gunzip.map { it[1] }
                                                             ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:65:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gtf = GUNZIP_GTF([[:], gtf]).gunzip.map { it[1] }
                                                           ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:71:85`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gff = GUNZIP_GFF([[:], file(gff, checkIfExists: true)]).gunzip.map { it[1] }
                                                                                      ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:73:81`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gff = channel.value(file(gff, checkIfExists: true)).map { [ [:], it ] }
                                                                                  ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:76:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_gtf = GFFREAD(ch_gff, []).gtf.map { it[1] }
                                                 ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:85:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_blacklist = GUNZIP_BLACKLIST([[:], blacklist]).gunzip.map { it[1] }
                                                                             ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:110:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gene_bed = GUNZIP_GENE_BED([[:], gene_bed]).gunzip.map { it[1] }
                                                                          ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:212:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_macs_gsize = KHMER_UNIQUEKMERS.out.kmers.map { meta, file ->
                                                            ^^^^
  ```

- Warning: `workflows/chipseq.nf:243:9`: Variable was declared but not used

  ```nextflow
          ch_transcriptome_bam = ALIGN_STAR.out.bam_transcript
          ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:247:9`: Variable was declared but not used

  ```nextflow
          ch_star_multiqc      = ALIGN_STAR.out.log_final
          ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:318:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      [ it[0], it[1], [] ]
                        ^^
  ```

- Warning: `workflows/chipseq.nf:318:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      [ it[0], it[1], [] ]
                               ^^
  ```

- Warning: `workflows/chipseq.nf:322:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      [ [:], it ]
                             ^^
  ```

- Warning: `workflows/chipseq.nf:326:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      [ [:], it ]
                             ^^
  ```

- Warning: `workflows/chipseq.nf:433:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, bams, bais ->
                          ^^^^
  ```

- Warning: `workflows/chipseq.nf:468:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, ip_bam, control_bam ->
                                ^^^^^^^^^^^
  ```

- Warning: `workflows/chipseq.nf:505:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              BAM_BEDGRAPH_BIGWIG_BEDTOOLS_UCSC.out.bigwig.collect{it[1]}.ifEmpty([]),
                                                                   ^^
  ```

- Warning: `workflows/chipseq.nf:506:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              BAM_PEAKS_CALL_QC_ANNOTATE_MACS3_HOMER.out.peaks.collect{it[1]}.ifEmpty([]),
                                                                       ^^
  ```

- Warning: `workflows/chipseq.nf:507:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_macs3_consensus_bed_lib.collect{it[1]}.ifEmpty([]),
                                                 ^^
  ```

- Warning: `workflows/chipseq.nf:508:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_macs3_consensus_txt_lib.collect{it[1]}.ifEmpty([])
                                                 ^^
  ```

- Warning: `workflows/chipseq.nf:550:69`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              FASTQ_FASTQC_UMITOOLS_TRIMGALORE.out.fastqc_zip.collect{it[1]}.ifEmpty([]),
                                                                      ^^
  ```

- Warning: `workflows/chipseq.nf:551:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              FASTQ_FASTQC_UMITOOLS_TRIMGALORE.out.trim_zip.collect{it[1]}.ifEmpty([]),
                                                                    ^^
  ```

- Warning: `workflows/chipseq.nf:552:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              FASTQ_FASTQC_UMITOOLS_TRIMGALORE.out.trim_log.collect{it[1]}.ifEmpty([]),
                                                                    ^^
  ```

- Warning: `workflows/chipseq.nf:554:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_samtools_stats.collect{it[1]}.ifEmpty([]),
                                        ^^
  ```

- Warning: `workflows/chipseq.nf:555:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_samtools_flagstat.collect{it[1]}.ifEmpty([]),
                                           ^^
  ```

- Warning: `workflows/chipseq.nf:556:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_samtools_idxstats.collect{it[1]}.ifEmpty([]),
                                           ^^
  ```

- Warning: `workflows/chipseq.nf:558:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              BAM_MARKDUPLICATES_PICARD.out.stats.collect{it[1]}.ifEmpty([]),
                                                          ^^
  ```

- Warning: `workflows/chipseq.nf:559:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              BAM_MARKDUPLICATES_PICARD.out.flagstat.collect{it[1]}.ifEmpty([]),
                                                             ^^
  ```

- Warning: `workflows/chipseq.nf:560:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              BAM_MARKDUPLICATES_PICARD.out.idxstats.collect{it[1]}.ifEmpty([]),
                                                             ^^
  ```

- Warning: `workflows/chipseq.nf:561:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              BAM_MARKDUPLICATES_PICARD.out.metrics.collect{it[1]}.ifEmpty([]),
                                                            ^^
  ```

- Warning: `workflows/chipseq.nf:563:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              BAM_FILTER_BAMTOOLS.out.stats.collect{it[1]}.ifEmpty([]),
                                                    ^^
  ```

- Warning: `workflows/chipseq.nf:564:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              BAM_FILTER_BAMTOOLS.out.flagstat.collect{it[1]}.ifEmpty([]),
                                                       ^^
  ```

- Warning: `workflows/chipseq.nf:565:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              BAM_FILTER_BAMTOOLS.out.idxstats.collect{it[1]}.ifEmpty([]),
                                                       ^^
  ```

- Warning: `workflows/chipseq.nf:566:61`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_picardcollectmultiplemetrics_multiqc.collect{it[1]}.ifEmpty([]),
                                                              ^^
  ```

- Warning: `workflows/chipseq.nf:568:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_preseq_multiqc.collect{it[1]}.ifEmpty([]),
                                        ^^
  ```

- Warning: `workflows/chipseq.nf:570:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_deeptoolsplotprofile_multiqc.collect{it[1]}.ifEmpty([]),
                                                      ^^
  ```

- Warning: `workflows/chipseq.nf:571:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_deeptoolsplotfingerprint_multiqc.collect{it[1]}.ifEmpty([]),
                                                          ^^
  ```

- Warning: `workflows/chipseq.nf:573:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_phantompeakqualtools_spp_multiqc.collect{it[1]}.ifEmpty([]),
                                                          ^^
  ```

- Warning: `workflows/chipseq.nf:574:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_phantompeakqualtools_nsc_multiqc.collect{it[1]}.ifEmpty([]),
                                                                  ^^
  ```

- Warning: `workflows/chipseq.nf:575:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_phantompeakqualtools_rsc_multiqc.collect{it[1]}.ifEmpty([]),
                                                                  ^^
  ```

- Warning: `workflows/chipseq.nf:576:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_phantompeakqualtools_correlation_multiqc.collect{it[1]}.ifEmpty([]),
                                                                          ^^
  ```

- Warning: `workflows/chipseq.nf:578:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              BAM_PEAKS_CALL_QC_ANNOTATE_MACS3_HOMER.out.frip_multiqc.collect{it[1]}.ifEmpty([]),
                                                                              ^^
  ```

- Warning: `workflows/chipseq.nf:579:83`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              BAM_PEAKS_CALL_QC_ANNOTATE_MACS3_HOMER.out.peak_count_multiqc.collect{it[1]}.ifEmpty([]),
                                                                                    ^^
  ```

- Warning: `workflows/chipseq.nf:581:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_subreadfeaturecounts_multiqc.collect{it[1]}.ifEmpty([]),
                                                      ^^
  ```
