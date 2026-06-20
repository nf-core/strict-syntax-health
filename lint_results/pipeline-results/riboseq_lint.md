# Nextflow lint results

- Generated: 2026-06-20T00:41:29.835162271Z
- Nextflow version: 26.05.0-edge
- Summary: 138 warnings

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

- Warning: `workflows/riboseq/main.nf:89:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_chrom_sizes      // channel: path(genome.sizes)
      ^^^^^^^^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:132:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_ribo_db = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:147:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:152:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:164:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              validateInputSamplesheet(it)
                                       ^^
  ```

- Warning: `workflows/riboseq/main.nf:240:103`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTQ_EQUALISE_READ_LENGTHS.out.riboseq_stats.collect{it[1]})
                                                                                                        ^^
  ```

- Warning: `workflows/riboseq/main.nf:250:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_star_index.map { [ [:], it ] },
                                     ^^
  ```

- Warning: `workflows/riboseq/main.nf:251:29`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_gtf.map { [ [:], it ] },
                              ^^
  ```

- Warning: `workflows/riboseq/main.nf:253:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta.map { [ [:], it ] },
                                ^^
  ```

- Warning: `workflows/riboseq/main.nf:254:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_transcript_fasta.map { [ [:], it ] }
                                           ^^
  ```

- Warning: `workflows/riboseq/main.nf:260:5`: Variable was declared but not used

  ```nextflow
      ch_transcriptome_bai       = FASTQ_ALIGN_STAR.out.bai_transcript
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:263:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .mix(FASTQ_ALIGN_STAR.out.stats.collect{it[1]})
                                                  ^^
  ```

- Warning: `workflows/riboseq/main.nf:264:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .mix(FASTQ_ALIGN_STAR.out.flagstat.collect{it[1]})
                                                     ^^
  ```

- Warning: `workflows/riboseq/main.nf:265:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .mix(FASTQ_ALIGN_STAR.out.idxstats.collect{it[1]})
                                                     ^^
  ```

- Warning: `workflows/riboseq/main.nf:266:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .mix(FASTQ_ALIGN_STAR.out.log_final.collect{it[1]})
                                                      ^^
  ```

- Warning: `workflows/riboseq/main.nf:276:35`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_fasta.map { [ [:], it ] },
                                    ^^
  ```

- Warning: `workflows/riboseq/main.nf:281:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_transcript_fasta.map { [ [:], it ] },
                                               ^^
  ```

- Warning: `workflows/riboseq/main.nf:302:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, bam, bai -> meta.strandedness in ['forward', 'reverse'] }
                              ^^^
  ```

- Warning: `workflows/riboseq/main.nf:302:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, bam, bai -> meta.strandedness in ['forward', 'reverse'] }
                                   ^^^
  ```

- Warning: `workflows/riboseq/main.nf:321:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      .filter { meta, bam -> meta.strandedness == 'unstranded' }
                                      ^^^
  ```

- Warning: `workflows/riboseq/main.nf:363:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_canonical_gtf.map { [ [:], it ] }.first()
                                            ^^
  ```

- Warning: `workflows/riboseq/main.nf:366:99`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(RIBOTISH_QUALITY_RIBOSEQ.out.distribution.collect{it[1]})
                                                                                                    ^^
  ```

- Warning: `workflows/riboseq/main.nf:386:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ribotish_predict_inputs.bam.map{meta, bam, bai -> [[id:'allsamples'], bam, bai]}.groupTuple(),
                                              ^^^^
  ```

- Warning: `workflows/riboseq/main.nf:390:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ribotish_predict_inputs.offset.map{meta, offset -> [[id:'allsamples'], offset]}.groupTuple(),
                                                 ^^^^
  ```

- Warning: `workflows/riboseq/main.nf:427:9`: Variable was declared but not used

  ```nextflow
      def orf_agreement_min_callers = enabled_orf_callers
          ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:430:5`: Variable was declared but not used

  ```nextflow
      ch_enabled_orf_callers      = Channel.value(enabled_orf_callers)
      ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:430:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_enabled_orf_callers      = Channel.value(enabled_orf_callers)
                                    ^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:431:5`: Variable was declared but not used

  ```nextflow
      ch_rank_aggregation_callers = Channel.value(rank_aggregation_callers)
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:431:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_rank_aggregation_callers = Channel.value(rank_aggregation_callers)
                                    ^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:444:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gtf.map { [ [:], it ] }.first()
                                  ^^
  ```

- Warning: `workflows/riboseq/main.nf:449:35`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_fasta.map { [ [:], it ] }.first(),
                                    ^^
  ```

- Warning: `workflows/riboseq/main.nf:465:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_ribocode_inputs.map { meta, bam, config -> [ meta, bam ] },
                                                  ^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:467:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_ribocode_inputs.map { meta, bam, config -> [ meta, config ] }
                                             ^^^
  ```

- Warning: `workflows/riboseq/main.nf:491:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gtf.map { [ [:], it ] },
                                  ^^
  ```

- Warning: `workflows/riboseq/main.nf:492:35`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_fasta.map { [ [:], it ] })
                                    ^^
  ```

- Warning: `workflows/riboseq/main.nf:495:89`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(RIBOWALTZ.out.ribowaltz_qc_data.collect{it[1]}.ifEmpty([]))
                                                                                          ^^
  ```

- Warning: `workflows/riboseq/main.nf:500:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          PLASTID_METAGENE_GENERATE(ch_canonical_gtf.map { [ [:], it ] })
                                                                  ^^
  ```

- Warning: `workflows/riboseq/main.nf:524:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_samplesheet.map { [ [:], it ] },
                                      ^^
  ```

- Warning: `workflows/riboseq/main.nf:538:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(QUANTIFY_STAR_SALMON.out.multiqc.collect{it[1]}.ifEmpty([]))
                                                                                       ^^
  ```

- Warning: `workflows/riboseq/main.nf:550:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, reads -> meta.sample_type in ['riboseq', 'rnaseq'] }
                              ^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:553:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_samplesheet.map { [ [:], it ] },
                                          ^^
  ```

- Warning: `workflows/riboseq/main.nf:567:88`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(QUANTIFY_PSEUDO_TE.out.multiqc.collect{it[1]}.ifEmpty([]))
                                                                                         ^^
  ```

- Warning: `workflows/riboseq/main.nf:592:67`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .collectFile(name: 'gene_inframe_psite_counts.tsv') { meta, file -> file }
                                                                    ^^^^
  ```

- Warning: `workflows/riboseq/main.nf:597:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .combine(QUANTIFY_STAR_SALMON.out.counts_gene_length_scaled.map{ meta, counts -> counts })
                                                                                   ^^^^
  ```

- Warning: `workflows/riboseq/main.nf:614:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it, it.variable, it.reference, it.target]}
                    ^^
  ```

- Warning: `workflows/riboseq/main.nf:614:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it, it.variable, it.reference, it.target]}
                        ^^
  ```

- Warning: `workflows/riboseq/main.nf:614:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it, it.variable, it.reference, it.target]}
                                     ^^
  ```

- Warning: `workflows/riboseq/main.nf:614:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it, it.variable, it.reference, it.target]}
                                                   ^^
  ```

- Warning: `workflows/riboseq/main.nf:618:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it[0], it[2], it[1]]}
                    ^^
  ```

- Warning: `workflows/riboseq/main.nf:618:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it[0], it[2], it[1]]}
                           ^^
  ```

- Warning: `workflows/riboseq/main.nf:618:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it[0], it[2], it[1]]}
                                  ^^
  ```

- Warning: `workflows/riboseq/main.nf:642:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_versions = ch_versions.filter{it != null}
                                       ^^
  ```

- Warning: `workflows/riboseq/main.nf:654:49`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_workflow_summary                   = Channel.value(paramsSummaryMultiqc(summary_params))
                                                  ^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:656:49`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_methods_description                = Channel.value(methodsDescriptionText(ch_multiqc_custom_methods_description))
                                                  ^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:698:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_multiqc_report = Channel.empty()
                              ^^^^^^^
  ```
