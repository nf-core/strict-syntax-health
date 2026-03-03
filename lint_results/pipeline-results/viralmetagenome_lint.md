# Nextflow lint results

- Generated: 2026-03-03T00:24:23.601791787Z
- Nextflow version: 26.02.0-edge
- Summary: 4 errors, 66 warnings

## :x: Errors

- Error: `conf/modules.config:16:170`: Unexpected input: '='

  ```nextflow
  save_final_reads            = params.save_final_reads ? (!params.skip_hostremoval ? 'host' : (!params.skip_complexity_filtering ? 'complexity' : (params.umi_deduplicate = 'read' ? 'deduplication' : 'trimming')))  : 'nothing'
                                                                                                                                                                           ^
  ```

- Error: `modules/nf-core/prinseqplusplus/main.nf:27:9`: `fasta` is already declared

  ```nextflow
      def fasta = fasta ? "-fastq ${fasta} -FASTA" : ''
          ^^^^^
  ```

- Error: `nextflow.config:104:39`: `mapper` is not defined

  ```nextflow
      intermediate_mapper             = mapper
                                        ^^^^^^
  ```

- Error: `nextflow.config:111:39`: `variant_caller` is not defined

  ```nextflow
      intermediate_variant_caller     = variant_caller
                                        ^^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `modules/local/blast_filter/main.nf:48:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/custom_mpileup/main.nf:39:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/custom_multiqc/main.nf:79:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/extract_cluster/main.nf:46:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/extract_precluster/main.nf:49:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/ivar_variants_to_vcf/main.nf:45:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/make_bed_mask/main.nf:50:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/make_bed_mask/main.nf:51:9`: Variable was declared but not used

  ```nextflow
      def args2 = task.ext.args2 ?: 5
          ^^^^^
  ```

- Warning: `modules/local/make_bed_mask/main.nf:53:9`: Variable was declared but not used

  ```nextflow
      def mpileup = save_mpileup ? "| tee ${prefix}.mpileup" : ""
          ^^^^^^^
  ```

- Warning: `modules/local/select_reference/main.nf:39:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/snpeff_build/main.nf:64:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/snpsift_extractfields/main.nf:55:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/consensus_qc/main.nf:21:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions        = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/consensus_qc/main.nf:22:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files   = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/consensus_qc/main.nf:23:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_blast           = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/consensus_qc/main.nf:24:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_checkv          = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/consensus_qc/main.nf:25:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_quast           = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/consensus_qc/main.nf:26:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_annotation      = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/consensus_qc/main.nf:27:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_genome_grouped  = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/consensus_qc/main.nf:31:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .collectFile(name: "all_genomes.fa") { it[1] }
                                                 ^^
  ```

- Warning: `subworkflows/local/consensus_qc/main.nf:46:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { id, genome, meta -> [meta, genome] }
                 ^^
  ```

- Warning: `subworkflows/local/fastq_fasta_iterative_consensus/main.nf:24:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_consensus_allsteps = Channel.empty()
                              ^^^^^^^
  ```

- Warning: `subworkflows/local/fastq_fasta_iterative_consensus/main.nf:25:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc = Channel.empty()
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/fastq_fasta_iterative_consensus/main.nf:26:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/fastq_fastqc_umitools_trimmomatic/main.nf:39:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/fastq_fastqc_umitools_trimmomatic/main.nf:40:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_fastqc_raw_html = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/fastq_fastqc_umitools_trimmomatic/main.nf:41:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_fastqc_raw_zip = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/fastq_fastqc_umitools_trimmomatic/main.nf:51:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_umi_log = Channel.empty()
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/fastq_fastqc_umitools_trimmomatic/main.nf:68:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_trim_summ           = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `subworkflows/local/fastq_fastqc_umitools_trimmomatic/main.nf:69:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_trim_unpaired_reads = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `subworkflows/local/fastq_fastqc_umitools_trimmomatic/main.nf:70:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_trim_log            = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `subworkflows/local/fastq_fastqc_umitools_trimmomatic/main.nf:71:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_fastqc_trim_html    = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `subworkflows/local/fastq_fastqc_umitools_trimmomatic/main.nf:72:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_fastqc_trim_zip     = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `subworkflows/local/fastq_fastqc_umitools_trimmomatic/main.nf:73:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_trim_read_count     = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `subworkflows/local/map_reads/main.nf:13:5`: Variable was declared but not used

  ```nextflow
      ch_reads = ch_reference_reads.map { meta, fasta, fastq -> [meta, fastq] }
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/map_reads/main.nf:13:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_reads = ch_reference_reads.map { meta, fasta, fastq -> [meta, fastq] }
                                                ^^^^^
  ```

- Warning: `subworkflows/local/map_reads/main.nf:14:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_reference = ch_reference_reads.map { meta, fasta, fastq -> [meta, fasta] }
                                                           ^^^^^
  ```

- Warning: `subworkflows/local/singleton_filtering/main.nf:12:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralmetagenome_pipeline/main.nf:29:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralmetagenome_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralmetagenome_pipeline/main.nf:95:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralmetagenome_pipeline/main.nf:326:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      return param ? Channel.fromPath(param, checkIfExists: true).collect() : []
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralmetagenome_pipeline/main.nf:330:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      return dbPath && skipFlag ? Channel.fromPath(dbPath, checkIfExists: true).map { db -> [[id: dbName], db] } : Channel.empty()
                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralmetagenome_pipeline/main.nf:330:114`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      return dbPath && skipFlag ? Channel.fromPath(dbPath, checkIfExists: true).map { db -> [[id: dbName], db] } : Channel.empty()
                                                                                                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralmetagenome_pipeline/main.nf:345:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, fasta, stats -> ["$meta.id\t$meta.sample\t$meta.cluster_id\t$meta.previous_step\t$stats.contig_size\t$stats.n_100"] }
                       ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralmetagenome_pipeline/main.nf:401:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, bam, mapped_reads ->
                       ^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralmetagenome_pipeline/main.nf:432:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, txt, fasta ->
                       ^^^
  ```

- Warning: `subworkflows/local/vcf_annotate/main.nf:12:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/viralmetagenome.nf:70:100`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def read_classifiers   = params.read_classifiers ? params.read_classifiers.split(',').collect{ it.trim().toLowerCase() } : []
                                                                                                     ^^
  ```

- Warning: `workflows/viralmetagenome.nf:71:112`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def contig_classifiers = params.precluster_classifiers ? params.precluster_classifiers.split(',').collect{ it.trim().toLowerCase() } : []
                                                                                                                 ^^
  ```

- Warning: `workflows/viralmetagenome.nf:78:5`: Variable was declared but not used

  ```nextflow
      ch_adapter_fasta   = createFileChannel(params.adapter_fasta)
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/viralmetagenome.nf:123:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_ref_pool         = ch_db.reference.collect{it[1]}.ifEmpty([]).map{it -> [[id: 'reference'], it]}
                                                        ^^
  ```

- Warning: `workflows/viralmetagenome.nf:124:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_annotation_db    = ch_db.annotation.collect{it[1]}.ifEmpty([]).map{it -> [[id: 'annotation'], it]}
                                                         ^^
  ```

- Warning: `workflows/viralmetagenome.nf:147:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_blast_refdb  = ch_blastdb_out.reference.collect{it[1]}.ifEmpty([]).map{it -> [[id: 'reference'], it]}
                                                             ^^
  ```

- Warning: `workflows/viralmetagenome.nf:163:95`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files        = ch_multiqc_files.mix(PREPROCESSING_ILLUMINA.out.mqc.collect{it[1]}.ifEmpty([]))
                                                                                                ^^
  ```

- Warning: `workflows/viralmetagenome.nf:177:84`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTQ_KRAKEN_KAIJU.out.mqc.collect{it[1]}.ifEmpty([]))
                                                                                     ^^
  ```

- Warning: `workflows/viralmetagenome.nf:236:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_clusters_summary    = FASTA_CONTIG_CLUST.out.clusters_summary.collect{it[1]}.ifEmpty([])
                                                                                       ^^
  ```

- Warning: `workflows/viralmetagenome.nf:237:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_clusters_tsv        = FASTA_CONTIG_CLUST.out.clusters_tsv.collect{it[1]}.ifEmpty([])
                                                                                   ^^
  ```

- Warning: `workflows/viralmetagenome.nf:349:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_mash_screen = FASTQ_FASTA_MASH_SCREEN.out.json.collect{it[1]}
                                                                    ^^
  ```

- Warning: `workflows/viralmetagenome.nf:411:83`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files      = ch_multiqc_files.mix(CONSENSUS_QC.out.mqc.collect{it[1]}.ifEmpty([]))
                                                                                    ^^
  ```

- Warning: `workflows/viralmetagenome.nf:412:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_checkv_summary     = CONSENSUS_QC.out.checkv.collect{it[1]}.ifEmpty([])
                                                                  ^^
  ```

- Warning: `workflows/viralmetagenome.nf:413:64`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_quast_summary      = CONSENSUS_QC.out.quast.collect{it[1]}.ifEmpty([])
                                                                 ^^
  ```

- Warning: `workflows/viralmetagenome.nf:414:64`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_blast_summary      = CONSENSUS_QC.out.blast.collect{it[1]}.ifEmpty([])
                                                                 ^^
  ```

- Warning: `workflows/viralmetagenome.nf:415:69`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_annotation_summary = CONSENSUS_QC.out.annotation.collect{it[1]}.ifEmpty([])
                                                                      ^^
  ```

- Warning: `workflows/viralmetagenome.nf:422:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_custom_config              = params.multiqc_config              ? channel.fromPath(params.multiqc_config, checkIfExists: true) : channel.empty()
      ^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/viralmetagenome.nf:423:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_logo                       = params.multiqc_logo                ? channel.fromPath(params.multiqc_logo, checkIfExists: true) : channel.empty()
      ^^^^^^^^^^^^^^^
  ```
