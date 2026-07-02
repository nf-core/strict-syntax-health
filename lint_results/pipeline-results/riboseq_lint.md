# Nextflow lint results

- Generated: 2026-07-02T00:41:15.622803911Z
- Nextflow version: 26.06.0-edge
- Summary: 160 warnings

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

- Warning: `conf/modules.config:759:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_align_intermeds || params.save_umi_intermeds ? it : null }
                                                                                       ^^
  ```

- Warning: `conf/modules.config:771:101`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_align_intermeds || params.with_umi || params.save_umi_intermeds ? it : null }
                                                                                                      ^^
  ```

- Warning: `conf/modules.config:793:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_align_intermeds || params.save_umi_intermeds ? it : null }
                                                                                   ^^
  ```

- Warning: `conf/modules.config:809:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_align_intermeds || params.save_umi_intermeds ? it : null }
                                                                                       ^^
  ```

- Warning: `conf/modules.config:820:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_align_intermeds || params.save_umi_intermeds ? it : null }
                                                                                   ^^
  ```

- Warning: `conf/modules.config:829:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_align_intermeds || params.save_umi_intermeds ? it : null }
                                                                                   ^^
  ```

- Warning: `conf/modules.config:839:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_align_intermeds || params.save_umi_intermeds ? it : null }
                                                                                   ^^
  ```

- Warning: `conf/modules.config:848:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_align_intermeds || params.save_umi_intermeds ? it : null }
                                                                                   ^^
  ```

- Warning: `conf/modules.config:1236:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_align_intermeds ? it : null }
                                                          ^^
  ```

- Warning: `conf/modules.config:1247:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_unaligned ? it : null }
                                                    ^^
  ```

- Warning: `conf/modules.config:1275:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_align_intermeds ? it : null }
                                                      ^^
  ```

- Warning: `main.nf:54:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `main.nf:88:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { checkMaxContigSize(it) }
                                        ^^
  ```

- Warning: `main.nf:94:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_samplesheet = Channel.value(file(params.input, checkIfExists: true))
                       ^^^^^^^
  ```

- Warning: `main.nf:96:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_contrasts_file = Channel.value(file(params.contrasts))
                              ^^^^^^^
  ```

- Warning: `main.nf:102:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_bowtie2_index = Channel.empty()
                         ^^^^^^^
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

- Warning: `subworkflows/local/coverage_tracks/main.nf:70:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      bigwig = UCSC_BEDGRAPHTOBIGWIG.out.bigwig // channel: [ val(meta), path(bigwig) ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/extended_orf_second_pass_align/main.nf:54:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_hybrid_star_index.map { [ [:], it ] },
                                            ^^
  ```

- Warning: `subworkflows/local/extended_orf_second_pass_align/main.nf:55:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_hybrid_gtf.map { [ [:], it ] },
                                     ^^
  ```

- Warning: `subworkflows/local/extended_orf_second_pass_align/main.nf:57:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta.map { [ [:], it ] },
                                ^^
  ```

- Warning: `subworkflows/local/extended_orf_second_pass_align/main.nf:58:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_hybrid_transcriptome_fasta.map { [ [:], it ] }
                                                     ^^
  ```

- Warning: `subworkflows/local/extended_orf_second_pass_align/main.nf:61:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = FASTQ_ALIGN_STAR_HYBRID.out.stats.collect{it[1]}
                                                                   ^^
  ```

- Warning: `subworkflows/local/extended_orf_second_pass_align/main.nf:62:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .mix(FASTQ_ALIGN_STAR_HYBRID.out.flagstat.collect{it[1]})
                                                            ^^
  ```

- Warning: `subworkflows/local/extended_orf_second_pass_align/main.nf:63:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .mix(FASTQ_ALIGN_STAR_HYBRID.out.idxstats.collect{it[1]})
                                                            ^^
  ```

- Warning: `subworkflows/local/extended_orf_second_pass_align/main.nf:64:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

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

- Warning: `subworkflows/local/novel_transcript_discovery/main.nf:77:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      hybrid_gtf = ch_hybrid_gtf // channel: path(hybrid.gtf) - canonical + filtered novel
      ^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/orf_caller_dispatch/main.nf:45:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions      = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/orf_caller_dispatch/main.nf:46:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/orf_caller_dispatch/main.nf:68:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_ribotish_predictions = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/orf_caller_dispatch/main.nf:72:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_canonical_gtf.map { [ [:], it ] }.first()
                                            ^^
  ```

- Warning: `subworkflows/local/orf_caller_dispatch/main.nf:75:99`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(RIBOTISH_QUALITY_RIBOSEQ.out.distribution.collect{it[1]})
                                                                                                    ^^
  ```

- Warning: `subworkflows/local/orf_caller_dispatch/main.nf:119:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_ribotricer_predictions = Channel.empty()
                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/orf_caller_dispatch/main.nf:143:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_rpbp_predictions = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/orf_caller_dispatch/main.nf:169:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_price_predictions = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/orf_caller_dispatch/main.nf:204:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_ribocode_predictions = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/orf_caller_dispatch/main.nf:229:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_ribocode_gtf_source.map { [ [id: ribocode_gtf_meta_id], it ] }.first()
                                                                         ^^
  ```

- Warning: `subworkflows/local/orf_caller_dispatch/main.nf:234:35`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_fasta.map { [ [:], it ] }.first(),
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

- Warning: `subworkflows/local/utils_nfcore_riboseq_pipeline/main.nf:31:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_riboseq_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_riboseq_pipeline/main.nf:142:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      hook_url        //  string: hook URL for notifications
      ^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_stringtie_merge/main.nf:29:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      stringtie_gtf = STRINGTIE_MERGE.out.merged_gtf // channel: [ meta, gtf ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
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

- Warning: `subworkflows/nf-core/utils_nextflow_pipeline/main.nf:43:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:20:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      valid_config
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:72:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:73:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_chrom_sizes      // channel: path(genome.sizes)
      ^^^^^^^^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:148:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              validateInputSamplesheet(it)
                                       ^^
  ```

- Warning: `workflows/riboseq/main.nf:224:103`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTQ_EQUALISE_READ_LENGTHS.out.riboseq_stats.collect{it[1]})
                                                                                                        ^^
  ```

- Warning: `workflows/riboseq/main.nf:234:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_star_index.map { [ [:], it ] },
                                     ^^
  ```

- Warning: `workflows/riboseq/main.nf:235:29`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_gtf.map { [ [:], it ] },
                              ^^
  ```

- Warning: `workflows/riboseq/main.nf:237:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta.map { [ [:], it ] },
                                ^^
  ```

- Warning: `workflows/riboseq/main.nf:238:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_transcript_fasta.map { [ [:], it ] }
                                           ^^
  ```

- Warning: `workflows/riboseq/main.nf:244:5`: Variable was declared but not used

  ```nextflow
      ch_transcriptome_bai       = FASTQ_ALIGN_STAR.out.bai_transcript
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:247:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .mix(FASTQ_ALIGN_STAR.out.stats.collect{it[1]})
                                                  ^^
  ```

- Warning: `workflows/riboseq/main.nf:248:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .mix(FASTQ_ALIGN_STAR.out.flagstat.collect{it[1]})
                                                     ^^
  ```

- Warning: `workflows/riboseq/main.nf:249:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .mix(FASTQ_ALIGN_STAR.out.idxstats.collect{it[1]})
                                                     ^^
  ```

- Warning: `workflows/riboseq/main.nf:250:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .mix(FASTQ_ALIGN_STAR.out.log_final.collect{it[1]})
                                                      ^^
  ```

- Warning: `workflows/riboseq/main.nf:260:35`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_fasta.map { [ [:], it ] },
                                    ^^
  ```

- Warning: `workflows/riboseq/main.nf:265:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_transcript_fasta.map { [ [:], it ] },
                                               ^^
  ```

- Warning: `workflows/riboseq/main.nf:376:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_fasta.map { [ [:], it ] },
                                        ^^
  ```

- Warning: `workflows/riboseq/main.nf:381:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  EXTENDED_ORF_SECOND_PASS_ALIGN.out.transcript_fasta.map { [ [:], it ] },
                                                                                   ^^
  ```

- Warning: `workflows/riboseq/main.nf:440:9`: Variable was declared but not used

  ```nextflow
      def orf_agreement_min_callers = enabled_orf_callers
          ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:443:5`: Variable was declared but not used

  ```nextflow
      ch_enabled_orf_callers      = channel.value(enabled_orf_callers)
      ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:444:5`: Variable was declared but not used

  ```nextflow
      ch_rank_aggregation_callers = channel.value(rank_aggregation_callers)
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:467:106`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(ORFTABLE_FASTA_GTF_BUILDORFCATALOGUE.out.multiqc.collect{it[1]}.ifEmpty([]))
                                                                                                           ^^
  ```

- Warning: `workflows/riboseq/main.nf:489:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gtf.map { [ [:], it ] },
                                  ^^
  ```

- Warning: `workflows/riboseq/main.nf:490:35`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_fasta.map { [ [:], it ] })
                                    ^^
  ```

- Warning: `workflows/riboseq/main.nf:493:89`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(RIBOWALTZ.out.ribowaltz_qc_data.collect{it[1]}.ifEmpty([]))
                                                                                          ^^
  ```

- Warning: `workflows/riboseq/main.nf:498:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          PLASTID_METAGENE_GENERATE(ch_canonical_gtf.map { [ [:], it ] })
                                                                  ^^
  ```

- Warning: `workflows/riboseq/main.nf:522:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_samplesheet.map { [ [:], it ] },
                                      ^^
  ```

- Warning: `workflows/riboseq/main.nf:536:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(QUANTIFY_STAR_SALMON.out.multiqc.collect{it[1]}.ifEmpty([]))
                                                                                       ^^
  ```

- Warning: `workflows/riboseq/main.nf:548:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, reads -> meta.sample_type in ['riboseq', 'rnaseq'] }
                              ^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:551:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_samplesheet.map { [ [:], it ] },
                                          ^^
  ```

- Warning: `workflows/riboseq/main.nf:565:88`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(QUANTIFY_PSEUDO_TE.out.multiqc.collect{it[1]}.ifEmpty([]))
                                                                                         ^^
  ```

- Warning: `workflows/riboseq/main.nf:590:67`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .collectFile(name: 'gene_inframe_psite_counts.tsv') { meta, file -> file }
                                                                    ^^^^
  ```

- Warning: `workflows/riboseq/main.nf:595:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .combine(QUANTIFY_STAR_SALMON.out.counts_gene_length_scaled.map{ meta, counts -> counts })
                                                                                   ^^^^
  ```

- Warning: `workflows/riboseq/main.nf:612:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it, it.variable, it.reference, it.target]}
                    ^^
  ```

- Warning: `workflows/riboseq/main.nf:612:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it, it.variable, it.reference, it.target]}
                        ^^
  ```

- Warning: `workflows/riboseq/main.nf:612:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it, it.variable, it.reference, it.target]}
                                     ^^
  ```

- Warning: `workflows/riboseq/main.nf:612:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it, it.variable, it.reference, it.target]}
                                                   ^^
  ```

- Warning: `workflows/riboseq/main.nf:616:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it[0], it[2], it[1]]}
                    ^^
  ```

- Warning: `workflows/riboseq/main.nf:616:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it[0], it[2], it[1]]}
                           ^^
  ```

- Warning: `workflows/riboseq/main.nf:616:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it[0], it[2], it[1]]}
                                  ^^
  ```

- Warning: `workflows/riboseq/main.nf:640:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_versions = ch_versions.filter{it != null}
                                       ^^
  ```
