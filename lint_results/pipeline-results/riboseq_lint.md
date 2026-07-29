# Nextflow lint results

- Generated: 2026-07-29T00:31:25.343012962Z
- Nextflow version: 26.07.0-edge
- Summary: 154 warnings

## :warning: Warnings

- Warning: `conf/modules.config:269:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_trimmed ? it : null }
                                                  ^^
  ```

- Warning: `conf/modules.config:296:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_trimmed ? it : null }
                                                  ^^
  ```

- Warning: `conf/modules.config:322:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_trimmed ? it : null }
                                              ^^
  ```

- Warning: `conf/modules.config:343:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_umi_intermeds ? it : null }
                                                        ^^
  ```

- Warning: `conf/modules.config:364:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_bbsplit_reads ? it : null }
                                                        ^^
  ```

- Warning: `conf/modules.config:381:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_non_ribo_reads ? it : null }
                                                         ^^
  ```

- Warning: `conf/modules.config:406:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_non_ribo_reads ? it : null }
                                                         ^^
  ```

- Warning: `conf/modules.config:437:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_non_ribo_reads ? it : null }
                                                     ^^
  ```

- Warning: `conf/modules.config:466:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_non_ribo_reads ? it : null }
                                                         ^^
  ```

- Warning: `conf/modules.config:526:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ) || params.save_align_intermeds || params.skip_markduplicates ? it : null }
                                                                                   ^^
  ```

- Warning: `conf/modules.config:600:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_align_intermeds ? it : null }
                                                          ^^
  ```

- Warning: `conf/modules.config:611:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_unaligned ? it : null }
                                                    ^^
  ```

- Warning: `conf/modules.config:844:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_align_intermeds || params.save_umi_intermeds ? it : null }
                                                                                       ^^
  ```

- Warning: `conf/modules.config:856:101`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_align_intermeds || params.with_umi || params.save_umi_intermeds ? it : null }
                                                                                                      ^^
  ```

- Warning: `conf/modules.config:878:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_align_intermeds || params.save_umi_intermeds ? it : null }
                                                                                   ^^
  ```

- Warning: `conf/modules.config:894:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_align_intermeds || params.save_umi_intermeds ? it : null }
                                                                                       ^^
  ```

- Warning: `conf/modules.config:905:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_align_intermeds || params.save_umi_intermeds ? it : null }
                                                                                   ^^
  ```

- Warning: `conf/modules.config:914:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_align_intermeds || params.save_umi_intermeds ? it : null }
                                                                                   ^^
  ```

- Warning: `conf/modules.config:924:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_align_intermeds || params.save_umi_intermeds ? it : null }
                                                                                   ^^
  ```

- Warning: `conf/modules.config:933:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_align_intermeds || params.save_umi_intermeds ? it : null }
                                                                                   ^^
  ```

- Warning: `conf/modules.config:1403:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_align_intermeds ? it : null }
                                                          ^^
  ```

- Warning: `conf/modules.config:1414:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_unaligned ? it : null }
                                                    ^^
  ```

- Warning: `conf/modules.config:1442:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_align_intermeds ? it : null }
                                                      ^^
  ```

- Warning: `main.nf:59:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `main.nf:93:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { checkMaxContigSize(it) }
                                        ^^
  ```

- Warning: `main.nf:99:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_samplesheet = Channel.value(file(params.input, checkIfExists: true))
                       ^^^^^^^
  ```

- Warning: `main.nf:101:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_contrasts_file = Channel.value(file(params.contrasts))
                              ^^^^^^^
  ```

- Warning: `main.nf:107:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_bowtie2_index = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `modules/local/dte_counts_prep/main.nf:22:5`: Variable was declared but not used

  ```nextflow
      args   = task.ext.args ?: ''
      ^^^^
  ```

- Warning: `modules/nf-core/custom/bed12codonpositions/main.nf:22:5`: Variable was declared but not used

  ```nextflow
      args   = task.ext.args ?: ''
      ^^^^
  ```

- Warning: `modules/nf-core/custom/orfcollapse/main.nf:29:5`: Variable was declared but not used

  ```nextflow
      args   = task.ext.args ?: ''
      ^^^^
  ```

- Warning: `modules/nf-core/custom/orfmerge/main.nf:28:5`: Variable was declared but not used

  ```nextflow
      args   = task.ext.args ?: ''
      ^^^^
  ```

- Warning: `modules/nf-core/custom/orfnormalise/main.nf:24:5`: Variable was declared but not used

  ```nextflow
      sample_id = meta.id ?: 'unknown'
      ^^^^^^^^^
  ```

- Warning: `modules/nf-core/custom/orfnormalise/main.nf:25:5`: Variable was declared but not used

  ```nextflow
      args      = task.ext.args ?: ''
      ^^^^
  ```

- Warning: `modules/nf-core/rpbp/getperiodiclengthsoffsets/main.nf:21:5`: Variable was declared but not used

  ```nextflow
      task_ext_args = task.ext.args ?: ''
      ^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/rpbp/preparegenome/main.nf:23:5`: Variable was declared but not used

  ```nextflow
      task_ext_args = task.ext.args ?: ''
      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/extended_orf_second_pass_align/main.nf:56:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_hybrid_star_index.map { [ [:], it ] },
                                            ^^
  ```

- Warning: `subworkflows/local/extended_orf_second_pass_align/main.nf:57:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_hybrid_gtf.map { [ [:], it ] },
                                     ^^
  ```

- Warning: `subworkflows/local/extended_orf_second_pass_align/main.nf:59:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta.map { [ [:], it, [] ] },
                                ^^
  ```

- Warning: `subworkflows/local/extended_orf_second_pass_align/main.nf:60:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_hybrid_transcriptome_fasta.map { [ [:], it, [] ] }
                                                     ^^
  ```

- Warning: `subworkflows/local/extended_orf_second_pass_align/main.nf:63:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = FASTQ_ALIGN_STAR_HYBRID.out.stats.collect{it[1]}
                                                                   ^^
  ```

- Warning: `subworkflows/local/extended_orf_second_pass_align/main.nf:64:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .mix(FASTQ_ALIGN_STAR_HYBRID.out.flagstat.collect{it[1]})
                                                            ^^
  ```

- Warning: `subworkflows/local/extended_orf_second_pass_align/main.nf:65:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .mix(FASTQ_ALIGN_STAR_HYBRID.out.idxstats.collect{it[1]})
                                                            ^^
  ```

- Warning: `subworkflows/local/extended_orf_second_pass_align/main.nf:66:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .mix(FASTQ_ALIGN_STAR_HYBRID.out.log_final.collect{it[1]})
                                                             ^^
  ```

- Warning: `subworkflows/local/fastq_equalise_read_lengths/main.nf:68:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, reads -> meta.pair != null }
                          ^^^^^
  ```

- Warning: `subworkflows/local/fastq_equalise_read_lengths/main.nf:69:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, reads -> meta.pair }
                       ^^^^^
  ```

- Warning: `subworkflows/local/fastq_equalise_read_lengths/main.nf:76:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, reads, pairs_needed ->
                          ^^^^^
  ```

- Warning: `subworkflows/local/fastq_equalise_read_lengths/main.nf:79:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, reads, pairs_needed -> [ meta, reads ] }
                              ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/fastq_equalise_read_lengths/main.nf:92:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def avg_len_idx = header.findIndexOf { it == 'avg_len' }
                                                         ^^
  ```

- Warning: `subworkflows/local/fastq_equalise_read_lengths/main.nf:103:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { pair, meta, reads, riboseq_trim_len ->
                 ^^^^
  ```

- Warning: `subworkflows/local/novel_transcript_discovery/main.nf:31:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_novel_pre_filter = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/novel_transcript_discovery/main.nf:34:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_novel_pre_filter = Channel
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/novel_transcript_discovery/main.nf:59:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ? Channel.fromPath(rrna_blacklist, checkIfExists: true).map { bed -> [ [id: 'rrna_blacklist'], bed ] }
            ^^^^^^^
  ```

- Warning: `subworkflows/local/novel_transcript_discovery/main.nf:60:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.empty()
            ^^^^^^^
  ```

- Warning: `subworkflows/local/novel_transcript_discovery/main.nf:70:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.value(gffcompare_class_codes),
          ^^^^^^^
  ```

- Warning: `subworkflows/local/orf_caller_dispatch/main.nf:47:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions      = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/orf_caller_dispatch/main.nf:48:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/orf_caller_dispatch/main.nf:70:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_ribotish_predictions = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/orf_caller_dispatch/main.nf:74:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_canonical_gtf.map { [ [:], it ] }
                                            ^^
  ```

- Warning: `subworkflows/local/orf_caller_dispatch/main.nf:77:99`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(RIBOTISH_QUALITY_RIBOSEQ.out.distribution.collect{it[1]})
                                                                                                    ^^
  ```

- Warning: `subworkflows/local/orf_caller_dispatch/main.nf:121:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_ribotricer_predictions = Channel.empty()
                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/orf_caller_dispatch/main.nf:145:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_rpbp_predictions = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/orf_caller_dispatch/main.nf:171:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_price_predictions = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/orf_caller_dispatch/main.nf:206:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_ribocode_predictions = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/orf_caller_dispatch/main.nf:231:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_ribocode_gtf_source.map { [ [id: ribocode_gtf_meta_id], it ] }
                                                                         ^^
  ```

- Warning: `subworkflows/local/orf_caller_dispatch/main.nf:236:35`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_fasta.map { [ [:], it ] },
                                    ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:59:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:65:68`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta    = GUNZIP_FASTA ( [ [:], fasta ] ).gunzip.map { it[1] }
                                                                     ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:67:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_fasta = Channel.value(file(fasta))
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:76:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_gtf      = GUNZIP_GTF ( [ [:], gtf ] ).gunzip.map { it[1] }
                                                                         ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:78:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ch_gtf = Channel.value(file(gtf))
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:85:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ch_gff = Channel.value(file(gff)).map { item -> [ [:], item ] }
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:87:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gtf = GFFREAD ( ch_gff, [] ).gtf.map { it[1] }
                                                        ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:120:95`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_add_fasta = GUNZIP_ADDITIONAL_FASTA ( [ [:], additional_fasta ] ).gunzip.map { it[1] }
                                                                                                ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:122:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_add_fasta = Channel.value(file(additional_fasta))
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:127:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_add_fasta.map{[[:], it]},
                                     ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:130:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta    = CUSTOM_CATADDITIONALFASTA.out.fasta.map{it[1]}.first()
                                                                ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:131:61`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_gtf      = CUSTOM_CATADDITIONALFASTA.out.gtf.map{it[1]}.first()
                                                              ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:143:93`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_canonical_gtf = GUNZIP_CANONICAL_GTF ( [ [:], canonical_gtf ] ).gunzip.map { it[1] }
                                                                                              ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:145:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_canonical_gtf = Channel.value(file(canonical_gtf))
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:152:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gtf.map { [ [id: it.baseName], it ] },
                                  ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:152:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gtf.map { [ [id: it.baseName], it ] },
                                                ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:159:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_canonical_gtf = GFFREAD_CANONICAL.out.gtf.map { it[1] }
                                                             ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:167:102`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_transcript_fasta = GUNZIP_TRANSCRIPT_FASTA ( [ [:], transcript_fasta ] ).gunzip.map { it[1] }
                                                                                                       ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:169:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_transcript_fasta = Channel.value(file(transcript_fasta))
                                    ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:183:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      SAMTOOLS_FAIDX ( ch_fasta.map { [ [:], it, [] ] }, true )
                                             ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:184:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_fai         = SAMTOOLS_FAIDX.out.fai.map { it[1] }
                                                    ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:185:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_chrom_sizes = SAMTOOLS_FAIDX.out.sizes.map { it[1] }
                                                      ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:197:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_bbsplit_index = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:201:95`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_bbsplit_index = UNTAR_BBSPLIT_INDEX ( [ [:], bbsplit_index ] ).untar.map { it[1] }
                                                                                                ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:203:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ch_bbsplit_index = Channel.value(file(bbsplit_index))
                                     ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:206:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              Channel
              ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:212:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .collect { [ it ] } // Collect entries as a list to pass as "tuple val(short_names), path(path_to_fasta)" to module
                               ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:222:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_sortmerna_index = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:223:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_rrna_fastas = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:228:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_rrna_fastas = Channel.from(ribo_db.readLines())
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:236:101`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_sortmerna_index = UNTAR_SORTMERNA_INDEX ( [ [:], sortmerna_index ] ).untar.map { it[1] }
                                                                                                      ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:238:38`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ch_sortmerna_index = Channel.value(file(sortmerna_index))
                                       ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:242:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  Channel.of([ [],[] ]),
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:243:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_rrna_fastas.collect().map { [ 'rrna_refs', it ] },
                                                                ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:244:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  Channel.of([ [],[] ])
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:253:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_star_index = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:257:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_star_index = UNTAR_STAR_INDEX ( [ [:], star_index ] ).untar.map { it[1] }
                                                                                       ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:259:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ch_star_index = Channel.value(file(star_index))
                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:272:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_star_index = STAR_GENOMEGENERATE ( ch_fasta.map { [ [:], it ] }, ch_gtf.map { [ [:], it ] } ).index.map { it[1] }
                                                                              ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:272:105`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_star_index = STAR_GENOMEGENERATE ( ch_fasta.map { [ [:], it ] }, ch_gtf.map { [ [:], it ] } ).index.map { it[1] }
                                                                                                          ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:272:126`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_star_index = STAR_GENOMEGENERATE ( ch_fasta.map { [ [:], it ] }, ch_gtf.map { [ [:], it ] } ).index.map { it[1] }
                                                                                                                               ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:280:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_salmon_index = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:283:88`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_salmon_index = UNTAR_SALMON_INDEX ( [ [:], salmon_index ] ).untar.map { it[1] }
                                                                                         ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:285:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_salmon_index = Channel.value(file(salmon_index))
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:296:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_salmon_index_te = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/quantify_orf_psite/main.nf:29:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/orftable_fasta_gtf_buildorfcatalogue/main.nf:51:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it.size() > 0 }
                    ^^
  ```

- Warning: `subworkflows/nf-core/orftable_fasta_gtf_buildorfcatalogue/main.nf:57:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it.size() > 0 }
                    ^^
  ```

- Warning: `workflows/riboseq/main.nf:85:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_chrom_sizes      // channel: path(genome.sizes)
      ^^^^^^^^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:160:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              validateInputSamplesheet(it)
                                       ^^
  ```

- Warning: `workflows/riboseq/main.nf:236:103`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTQ_EQUALISE_READ_LENGTHS.out.riboseq_stats.collect{it[1]})
                                                                                                        ^^
  ```

- Warning: `workflows/riboseq/main.nf:245:64`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_transcript_fasta_fai = ch_transcript_fasta.map { [ [:], it, [] ] }
                                                                 ^^
  ```

- Warning: `workflows/riboseq/main.nf:249:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_star_index.map { [ [:], it ] },
                                     ^^
  ```

- Warning: `workflows/riboseq/main.nf:250:29`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_gtf.map { [ [:], it ] },
                              ^^
  ```

- Warning: `workflows/riboseq/main.nf:259:5`: Variable was declared but not used

  ```nextflow
      ch_transcriptome_bai       = FASTQ_ALIGN_STAR.out.index_transcript
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:262:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .mix(FASTQ_ALIGN_STAR.out.stats.collect{it[1]})
                                                  ^^
  ```

- Warning: `workflows/riboseq/main.nf:263:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .mix(FASTQ_ALIGN_STAR.out.flagstat.collect{it[1]})
                                                     ^^
  ```

- Warning: `workflows/riboseq/main.nf:264:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .mix(FASTQ_ALIGN_STAR.out.idxstats.collect{it[1]})
                                                     ^^
  ```

- Warning: `workflows/riboseq/main.nf:265:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .mix(FASTQ_ALIGN_STAR.out.log_final.collect{it[1]})
                                                      ^^
  ```

- Warning: `workflows/riboseq/main.nf:394:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  EXTENDED_ORF_SECOND_PASS_ALIGN.out.transcript_fasta.map { [ [:], it, [] ] },
                                                                                   ^^
  ```

- Warning: `workflows/riboseq/main.nf:467:9`: Variable was declared but not used

  ```nextflow
      def orf_agreement_min_callers = enabled_orf_callers
          ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:470:5`: Variable was declared but not used

  ```nextflow
      ch_enabled_orf_callers      = channel.value(enabled_orf_callers)
      ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:471:5`: Variable was declared but not used

  ```nextflow
      ch_rank_aggregation_callers = channel.value(rank_aggregation_callers)
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:494:106`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(ORFTABLE_FASTA_GTF_BUILDORFCATALOGUE.out.multiqc.collect{it[1]}.ifEmpty([]))
                                                                                                           ^^
  ```

- Warning: `workflows/riboseq/main.nf:516:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gtf.map { [ [:], it ] },
                                  ^^
  ```

- Warning: `workflows/riboseq/main.nf:517:35`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_fasta.map { [ [:], it ] })
                                    ^^
  ```

- Warning: `workflows/riboseq/main.nf:520:89`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(RIBOWALTZ.out.ribowaltz_qc_data.collect{it[1]}.ifEmpty([]))
                                                                                          ^^
  ```

- Warning: `workflows/riboseq/main.nf:525:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_orf_count_matrix = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:529:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          PLASTID_METAGENE_GENERATE(ch_canonical_gtf.map { [ [:], it ] })
                                                                  ^^
  ```

- Warning: `workflows/riboseq/main.nf:571:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_samplesheet.map { [ [:], it ] },
                                      ^^
  ```

- Warning: `workflows/riboseq/main.nf:585:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(QUANTIFY_STAR_SALMON.out.multiqc.collect{it[1]}.ifEmpty([]))
                                                                                       ^^
  ```

- Warning: `workflows/riboseq/main.nf:597:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, reads -> meta.sample_type in ['riboseq', 'rnaseq'] }
                              ^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:600:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_samplesheet.map { [ [:], it ] },
                                          ^^
  ```

- Warning: `workflows/riboseq/main.nf:614:88`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(QUANTIFY_PSEUDO_TE.out.multiqc.collect{it[1]}.ifEmpty([]))
                                                                                         ^^
  ```

- Warning: `workflows/riboseq/main.nf:639:67`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .collectFile(name: 'gene_inframe_psite_counts.tsv') { meta, file -> file }
                                                                    ^^^^
  ```

- Warning: `workflows/riboseq/main.nf:644:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .combine(QUANTIFY_STAR_SALMON.out.counts_gene_length_scaled.map{ meta, counts -> counts })
                                                                                   ^^^^
  ```

- Warning: `workflows/riboseq/main.nf:675:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it, it.variable, it.reference, it.target]}
                    ^^
  ```

- Warning: `workflows/riboseq/main.nf:675:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it, it.variable, it.reference, it.target]}
                        ^^
  ```

- Warning: `workflows/riboseq/main.nf:675:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it, it.variable, it.reference, it.target]}
                                     ^^
  ```

- Warning: `workflows/riboseq/main.nf:675:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it, it.variable, it.reference, it.target]}
                                                   ^^
  ```

- Warning: `workflows/riboseq/main.nf:679:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it[0], it[2], it[1]]}
                    ^^
  ```

- Warning: `workflows/riboseq/main.nf:679:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it[0], it[2], it[1]]}
                           ^^
  ```

- Warning: `workflows/riboseq/main.nf:679:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it[0], it[2], it[1]]}
                                  ^^
  ```

- Warning: `workflows/riboseq/main.nf:727:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_full_hybrid_gtf.map { [ [:], it ] },
                                                  ^^
  ```

- Warning: `workflows/riboseq/main.nf:730:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_full_hybrid_transcript_fasta.map { [ [:], it, [] ] }
                                                               ^^
  ```

- Warning: `workflows/riboseq/main.nf:742:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      ch_full_hybrid_transcript_fasta.map { [ [:], it, [] ] },
                                                                   ^^
  ```

- Warning: `workflows/riboseq/main.nf:749:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_samplesheet.map { [ [:], it ] },
                                              ^^
  ```

- Warning: `workflows/riboseq/main.nf:809:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_versions = ch_versions.filter{it != null}
                                       ^^
  ```
