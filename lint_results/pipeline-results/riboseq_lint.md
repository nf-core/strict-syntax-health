# Nextflow lint results

- Generated: 2026-05-01T00:35:57.980724738Z
- Nextflow version: 26.04.0
- Summary: 124 warnings

## :warning: Warnings

- Warning: `conf/modules.config:256:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_trimmed ? it : null }
                                                  ^^
  ```

- Warning: `conf/modules.config:283:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_trimmed ? it : null }
                                                  ^^
  ```

- Warning: `conf/modules.config:309:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_trimmed ? it : null }
                                              ^^
  ```

- Warning: `conf/modules.config:330:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_umi_intermeds ? it : null }
                                                        ^^
  ```

- Warning: `conf/modules.config:351:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_bbsplit_reads ? it : null }
                                                        ^^
  ```

- Warning: `conf/modules.config:368:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_non_ribo_reads ? it : null }
                                                         ^^
  ```

- Warning: `conf/modules.config:393:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_non_ribo_reads ? it : null }
                                                         ^^
  ```

- Warning: `conf/modules.config:424:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_non_ribo_reads ? it : null }
                                                     ^^
  ```

- Warning: `conf/modules.config:453:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_non_ribo_reads ? it : null }
                                                         ^^
  ```

- Warning: `conf/modules.config:513:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ) || params.save_align_intermeds || params.skip_markduplicates ? it : null }
                                                                                   ^^
  ```

- Warning: `conf/modules.config:587:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_align_intermeds ? it : null }
                                                          ^^
  ```

- Warning: `conf/modules.config:598:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_unaligned ? it : null }
                                                    ^^
  ```

- Warning: `conf/modules.config:746:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_align_intermeds || params.save_umi_intermeds ? it : null }
                                                                                       ^^
  ```

- Warning: `conf/modules.config:758:101`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_align_intermeds || params.with_umi || params.save_umi_intermeds ? it : null }
                                                                                                      ^^
  ```

- Warning: `conf/modules.config:780:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_align_intermeds || params.save_umi_intermeds ? it : null }
                                                                                   ^^
  ```

- Warning: `conf/modules.config:796:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_align_intermeds || params.save_umi_intermeds ? it : null }
                                                                                       ^^
  ```

- Warning: `conf/modules.config:807:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_align_intermeds || params.save_umi_intermeds ? it : null }
                                                                                   ^^
  ```

- Warning: `conf/modules.config:816:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_align_intermeds || params.save_umi_intermeds ? it : null }
                                                                                   ^^
  ```

- Warning: `conf/modules.config:826:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_align_intermeds || params.save_umi_intermeds ? it : null }
                                                                                   ^^
  ```

- Warning: `conf/modules.config:835:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_align_intermeds || params.save_umi_intermeds ? it : null }
                                                                                   ^^
  ```

- Warning: `main.nf:54:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `main.nf:87:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { checkMaxContigSize(it) }
                                        ^^
  ```

- Warning: `main.nf:93:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_samplesheet = Channel.value(file(params.input, checkIfExists: true))
                       ^^^^^^^
  ```

- Warning: `main.nf:95:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_contrasts_file = Channel.value(file(params.contrasts))
                              ^^^^^^^
  ```

- Warning: `main.nf:101:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

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

- Warning: `subworkflows/local/prepare_genome/main.nf:56:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:62:68`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta    = GUNZIP_FASTA ( [ [:], fasta ] ).gunzip.map { it[1] }
                                                                     ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:64:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_fasta = Channel.value(file(fasta))
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:73:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_gtf      = GUNZIP_GTF ( [ [:], gtf ] ).gunzip.map { it[1] }
                                                                         ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:75:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ch_gtf = Channel.value(file(gtf))
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:82:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ch_gff = Channel.value(file(gff)).map { item -> [ [:], item ] }
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:84:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gtf = GFFREAD ( ch_gff, [] ).gtf.map { it[1] }
                                                        ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:114:95`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_add_fasta = GUNZIP_ADDITIONAL_FASTA ( [ [:], additional_fasta ] ).gunzip.map { it[1] }
                                                                                                ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:116:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_add_fasta = Channel.value(file(additional_fasta))
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:121:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_add_fasta.map{[[:], it]},
                                     ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:124:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta    = CUSTOM_CATADDITIONALFASTA.out.fasta.map{it[1]}.first()
                                                                ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:125:61`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_gtf      = CUSTOM_CATADDITIONALFASTA.out.gtf.map{it[1]}.first()
                                                              ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:134:102`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_transcript_fasta = GUNZIP_TRANSCRIPT_FASTA ( [ [:], transcript_fasta ] ).gunzip.map { it[1] }
                                                                                                       ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:136:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_transcript_fasta = Channel.value(file(transcript_fasta))
                                    ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:150:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      SAMTOOLS_FAIDX ( ch_fasta.map { [ [:], it, [] ] }, true )
                                             ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:151:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_fai         = SAMTOOLS_FAIDX.out.fai.map { it[1] }
                                                    ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:152:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_chrom_sizes = SAMTOOLS_FAIDX.out.sizes.map { it[1] }
                                                      ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:164:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_bbsplit_index = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:168:95`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_bbsplit_index = UNTAR_BBSPLIT_INDEX ( [ [:], bbsplit_index ] ).untar.map { it[1] }
                                                                                                ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:170:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ch_bbsplit_index = Channel.value(file(bbsplit_index))
                                     ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:173:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              Channel
              ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:179:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .collect { [ it ] } // Collect entries as a list to pass as "tuple val(short_names), path(path_to_fasta)" to module
                               ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:189:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_sortmerna_index = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:190:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_rrna_fastas = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:195:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_rrna_fastas = Channel.from(ribo_db.readLines())
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:203:101`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_sortmerna_index = UNTAR_SORTMERNA_INDEX ( [ [:], sortmerna_index ] ).untar.map { it[1] }
                                                                                                      ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:205:38`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ch_sortmerna_index = Channel.value(file(sortmerna_index))
                                       ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:209:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  Channel.of([ [],[] ]),
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:210:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_rrna_fastas.collect().map { [ 'rrna_refs', it ] },
                                                                ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:211:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  Channel.of([ [],[] ])
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:220:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_star_index = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:224:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_star_index = UNTAR_STAR_INDEX ( [ [:], star_index ] ).untar.map { it[1] }
                                                                                       ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:226:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ch_star_index = Channel.value(file(star_index))
                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:239:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_star_index = STAR_GENOMEGENERATE ( ch_fasta.map { [ [:], it ] }, ch_gtf.map { [ [:], it ] } ).index.map { it[1] }
                                                                              ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:239:105`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_star_index = STAR_GENOMEGENERATE ( ch_fasta.map { [ [:], it ] }, ch_gtf.map { [ [:], it ] } ).index.map { it[1] }
                                                                                                          ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:239:126`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_star_index = STAR_GENOMEGENERATE ( ch_fasta.map { [ [:], it ] }, ch_gtf.map { [ [:], it ] } ).index.map { it[1] }
                                                                                                                               ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:247:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_salmon_index = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:250:88`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_salmon_index = UNTAR_SALMON_INDEX ( [ [:], salmon_index ] ).untar.map { it[1] }
                                                                                         ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:252:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_salmon_index = Channel.value(file(salmon_index))
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:263:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

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

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:88:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_chrom_sizes      // channel: path(genome.sizes)
      ^^^^^^^^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:131:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_ribo_db = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:146:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:151:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:163:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              validateInputSamplesheet(it)
                                       ^^
  ```

- Warning: `workflows/riboseq/main.nf:239:103`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTQ_EQUALISE_READ_LENGTHS.out.riboseq_stats.collect{it[1]})
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

- Warning: `workflows/riboseq/main.nf:252:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta.map { [ [:], it ] },
                                ^^
  ```

- Warning: `workflows/riboseq/main.nf:253:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_transcript_fasta.map { [ [:], it ] }
                                           ^^
  ```

- Warning: `workflows/riboseq/main.nf:259:5`: Variable was declared but not used

  ```nextflow
      ch_transcriptome_bai       = FASTQ_ALIGN_STAR.out.bai_transcript
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

- Warning: `workflows/riboseq/main.nf:275:35`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_fasta.map { [ [:], it ] },
                                    ^^
  ```

- Warning: `workflows/riboseq/main.nf:280:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_transcript_fasta.map { [ [:], it ] },
                                               ^^
  ```

- Warning: `workflows/riboseq/main.nf:301:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, bam, bai -> meta.strandedness in ['forward', 'reverse'] }
                              ^^^
  ```

- Warning: `workflows/riboseq/main.nf:301:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, bam, bai -> meta.strandedness in ['forward', 'reverse'] }
                                   ^^^
  ```

- Warning: `workflows/riboseq/main.nf:320:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      .filter { meta, bam -> meta.strandedness == 'unstranded' }
                                      ^^^
  ```

- Warning: `workflows/riboseq/main.nf:358:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gtf.map { [ [:], it ] }.first()
                                  ^^
  ```

- Warning: `workflows/riboseq/main.nf:361:99`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(RIBOTISH_QUALITY_RIBOSEQ.out.distribution.collect{it[1]})
                                                                                                    ^^
  ```

- Warning: `workflows/riboseq/main.nf:381:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ribotish_predict_inputs.bam.map{meta, bam, bai -> [[id:'allsamples'], bam, bai]}.groupTuple(),
                                              ^^^^
  ```

- Warning: `workflows/riboseq/main.nf:385:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ribotish_predict_inputs.offset.map{meta, offset -> [[id:'allsamples'], offset]}.groupTuple(),
                                                 ^^^^
  ```

- Warning: `workflows/riboseq/main.nf:415:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gtf.map { [ [:], it ] }.first()
                                  ^^
  ```

- Warning: `workflows/riboseq/main.nf:420:35`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_fasta.map { [ [:], it ] }.first(),
                                    ^^
  ```

- Warning: `workflows/riboseq/main.nf:436:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_ribocode_inputs.map { meta, bam, config -> [ meta, bam ] },
                                                  ^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:438:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_ribocode_inputs.map { meta, bam, config -> [ meta, config ] }
                                             ^^^
  ```

- Warning: `workflows/riboseq/main.nf:462:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gtf.map { [ [:], it ] },
                                  ^^
  ```

- Warning: `workflows/riboseq/main.nf:463:35`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_fasta.map { [ [:], it ] })
                                    ^^
  ```

- Warning: `workflows/riboseq/main.nf:470:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          PLASTID_METAGENE_GENERATE(ch_gtf.map { [ [:], it ] })
                                                        ^^
  ```

- Warning: `workflows/riboseq/main.nf:492:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_samplesheet.map { [ [:], it ] },
                                      ^^
  ```

- Warning: `workflows/riboseq/main.nf:506:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(QUANTIFY_STAR_SALMON.out.multiqc.collect{it[1]}.ifEmpty([]))
                                                                                       ^^
  ```

- Warning: `workflows/riboseq/main.nf:518:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, reads -> meta.sample_type in ['riboseq', 'rnaseq'] }
                              ^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:521:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_samplesheet.map { [ [:], it ] },
                                          ^^
  ```

- Warning: `workflows/riboseq/main.nf:535:88`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(QUANTIFY_PSEUDO_TE.out.multiqc.collect{it[1]}.ifEmpty([]))
                                                                                         ^^
  ```

- Warning: `workflows/riboseq/main.nf:560:67`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .collectFile(name: 'gene_inframe_psite_counts.tsv') { meta, file -> file }
                                                                    ^^^^
  ```

- Warning: `workflows/riboseq/main.nf:565:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .combine(QUANTIFY_STAR_SALMON.out.counts_gene_length_scaled.map{ meta, counts -> counts })
                                                                                   ^^^^
  ```

- Warning: `workflows/riboseq/main.nf:582:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it, it.variable, it.reference, it.target]}
                    ^^
  ```

- Warning: `workflows/riboseq/main.nf:582:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it, it.variable, it.reference, it.target]}
                        ^^
  ```

- Warning: `workflows/riboseq/main.nf:582:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it, it.variable, it.reference, it.target]}
                                     ^^
  ```

- Warning: `workflows/riboseq/main.nf:582:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it, it.variable, it.reference, it.target]}
                                                   ^^
  ```

- Warning: `workflows/riboseq/main.nf:586:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it[0], it[2], it[1]]}
                    ^^
  ```

- Warning: `workflows/riboseq/main.nf:586:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it[0], it[2], it[1]]}
                           ^^
  ```

- Warning: `workflows/riboseq/main.nf:586:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it[0], it[2], it[1]]}
                                  ^^
  ```

- Warning: `workflows/riboseq/main.nf:610:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_versions = ch_versions.filter{it != null}
                                       ^^
  ```

- Warning: `workflows/riboseq/main.nf:622:49`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_workflow_summary                   = Channel.value(paramsSummaryMultiqc(summary_params))
                                                  ^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:624:49`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_methods_description                = Channel.value(methodsDescriptionText(ch_multiqc_custom_methods_description))
                                                  ^^^^^^^
  ```

- Warning: `workflows/riboseq/main.nf:666:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_multiqc_report = Channel.empty()
                              ^^^^^^^
  ```
