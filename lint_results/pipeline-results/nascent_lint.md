# Nextflow lint results

- Generated: 2026-07-10T00:36:20.868864430Z
- Nextflow version: 26.06.0-edge
- Summary: 5 errors, 158 warnings

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

- Error: `tests/config/test_data.config:3:1`: Variable declarations cannot be mixed with config statements

  ```nextflow
  def nf_core_nascent_data = "https://raw.githubusercontent.com/nf-core/test-datasets/nascent"
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `tests/config/test_data.config:5:1`: Try-catch blocks cannot be mixed with config statements

  ```nextflow
  try {
  ^
  ```

- Error: `tests/config/test_data.config:16:45`: `nf_core_nascent_data` is not defined

  ```nextflow
              tune_csv                   = "${nf_core_nascent_data}/misc/tune.csv"
                                              ^^^^^^^^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `conf/modules.config:136:29`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def parts = it.trim().split(/\s+/, 2)
                              ^^
  ```

- Warning: `conf/modules.config:140:29`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def parts = it.trim().split(/\s+/, 2)
                              ^^
  ```

- Warning: `main.nf:75:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = NASCENT.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/bowtie2/align/main.nf:93:9`: Variable was declared but not used

  ```nextflow
      def reference = fasta && extension=="cram"  ? "--reference ${fasta}" : ""
          ^^^^^^^^^
  ```

- Warning: `modules/nf-core/bwa/mem/main.nf:56:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/bwa/mem/main.nf:59:9`: Variable was declared but not used

  ```nextflow
      def samtools_command = sort_bam ? 'sort' : 'view'
          ^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/bwamem2/mem/main.nf:59:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/bwamem2/mem/main.nf:62:9`: Variable was declared but not used

  ```nextflow
      def samtools_command = sort_bam ? 'sort' : 'view'
          ^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/bwamem2/mem/main.nf:66:9`: Variable was declared but not used

  ```nextflow
      def reference = fasta && extension=="cram"  ? "--reference ${fasta}" : ""
          ^^^^^^^^^
  ```

- Warning: `modules/nf-core/cat/cat/main.nf:23:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def file_list = files_in.collect { it.toString() }
                                         ^^
  ```

- Warning: `modules/nf-core/cat/cat/main.nf:58:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def file_list   = files_in.collect { it.toString() }
                                           ^^
  ```

- Warning: `modules/nf-core/cat/fastq/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/cat/fastq/main.nf:23:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def readList = reads instanceof List ? reads.collect{ it.toString() } : [reads.toString()]
                                                            ^^
  ```

- Warning: `modules/nf-core/cat/fastq/main.nf:54:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def readList = reads instanceof List ? reads.collect{ it.toString() } : [reads.toString()]
                                                            ^^
  ```

- Warning: `modules/nf-core/custom/getchromsizes/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/deeptools/bamcoverage/main.nf:69:9`: Variable was declared but not used

  ```nextflow
      def extension = args.contains("--outFileFormat bedgraph") || args.contains("-of bedgraph") ? ".bedgraph" : ".bigWig"
          ^^^^^^^^^
  ```

- Warning: `modules/nf-core/dragmap/align/main.nf:58:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/dragmap/align/main.nf:61:9`: Variable was declared but not used

  ```nextflow
      def reads_command = meta.single_end ? "-1 $reads" : "-1 ${reads[0]} -2 ${reads[1]}"
          ^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/dragmap/align/main.nf:62:9`: Variable was declared but not used

  ```nextflow
      def samtools_command = sort_bam ? 'sort' : 'view'
          ^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/dragmap/align/main.nf:66:9`: Variable was declared but not used

  ```nextflow
      def reference = fasta && extension=="cram"  ? "--reference ${fasta}" : ""
          ^^^^^^^^^
  ```

- Warning: `modules/nf-core/gffread/main.nf:26:103`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def extension   = args.contains("-T")       ? 'gtf' : ( ( ['-w', '-x', '-y' ].any { args.contains(it) } ) ? 'fasta' : 'gff3' )
                                                                                                        ^^
  ```

- Warning: `modules/nf-core/gffread/main.nf:30:61`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def args_sorted = args.replaceAll(/(.*)(-[wxy])(.*)/) { all, pre, param, post -> "$pre $post $param" }.trim()
                                                              ^^^
  ```

- Warning: `modules/nf-core/gffread/main.nf:49:103`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def extension   = args.contains("-T")       ? 'gtf' : ( ( ['-w', '-x', '-y' ].any { args.contains(it) } ) ? 'fasta' : 'gff3' )
                                                                                                        ^^
  ```

- Warning: `modules/nf-core/gunzip/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/homer/pos2bed/main.nf:20:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/rseqc/readdistribution/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/rseqc/tin/main.nf:24:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/rseqc/tin/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/star/align/main.nf:45:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      meta.single_end ? [reads].flatten().each{reads1 << it} : reads.eachWithIndex{ v, ix -> ( ix & 1 ? reads2 : reads1) << v }
                                                         ^^
  ```

- Warning: `modules/nf-core/unzip/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/align_bwamem2/main.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/align_dragmap/main.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/coverage_graphs/main.nf:13:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      sizes
      ^^^^^
  ```

- Warning: `subworkflows/local/coverage_graphs/main.nf:19:5`: Variable was declared but not used

  ```nextflow
      bam = bam_bai.map { [it[0], it[1]] }
      ^^^
  ```

- Warning: `subworkflows/local/coverage_graphs/main.nf:19:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      bam = bam_bai.map { [it[0], it[1]] }
                           ^^
  ```

- Warning: `subworkflows/local/coverage_graphs/main.nf:19:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      bam = bam_bai.map { [it[0], it[1]] }
                                  ^^
  ```

- Warning: `subworkflows/local/coverage_graphs/main.nf:21:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/dreg_prep/main.nf:6:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      bai
      ^^^
  ```

- Warning: `subworkflows/local/dreg_prep/main.nf:7:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      sizes
      ^^^^^
  ```

- Warning: `subworkflows/local/grohmm/main.nf:20:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome.nf:36:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      hisat2_index
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome.nf:40:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome.nf:46:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta = GUNZIP_FASTA([[:], fasta]).gunzip.map { it[1] }
                                                             ^^
  ```

- Warning: `subworkflows/local/prepare_genome.nf:50:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_fasta = Channel.value(file(fasta))
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome.nf:59:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_gtf = GUNZIP_GTF([[:], gtf]).gunzip.map { it[1] }
                                                               ^^
  ```

- Warning: `subworkflows/local/prepare_genome.nf:63:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ch_gtf = Channel.value(file(gtf))
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome.nf:74:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gtf = GFFREAD(ch_gff, ch_fasta).gtf.map { it[1] }
                                                           ^^
  ```

- Warning: `subworkflows/local/prepare_genome.nf:84:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gene_bed = GUNZIP_GENE_BED([[:], gene_bed]).gunzip.map { it[1] }
                                                                          ^^
  ```

- Warning: `subworkflows/local/prepare_genome.nf:99:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      CUSTOM_GETCHROMSIZES(ch_fasta.map { [[:], it] })
                                                ^^
  ```

- Warning: `subworkflows/local/prepare_genome.nf:100:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_fai = CUSTOM_GETCHROMSIZES.out.fai.map { it[1] }
                                                  ^^
  ```

- Warning: `subworkflows/local/prepare_genome.nf:101:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_chrom_sizes = CUSTOM_GETCHROMSIZES.out.sizes.map { it[1] }
                                                            ^^
  ```

- Warning: `subworkflows/local/prepare_genome.nf:107:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_bwa_index = Channel.empty()
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome.nf:108:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_dragmap = Channel.empty()
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome.nf:109:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_bowtie2_index = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome.nf:123:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_bwa_index = BWA_INDEX(ch_fasta.map { [[:], it] }).index
                                                            ^^
  ```

- Warning: `subworkflows/local/prepare_genome.nf:139:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_bwa_index = BWAMEM2_INDEX(ch_fasta.map { [[:], it] }).index
                                                                ^^
  ```

- Warning: `subworkflows/local/prepare_genome.nf:155:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_dragmap = DRAGMAP_HASHTABLE(ch_fasta.map { [[:], it] }).hashmap
                                                                  ^^
  ```

- Warning: `subworkflows/local/prepare_genome.nf:171:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_bowtie2_index = BOWTIE2_BUILD(ch_fasta.map { [[:], it] }).index
                                                                    ^^
  ```

- Warning: `subworkflows/local/quality_control.nf:14:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      bam = bam_bai.map { [it[0], it[1]] }
                           ^^
  ```

- Warning: `subworkflows/local/quality_control.nf:14:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      bam = bam_bai.map { [it[0], it[1]] }
                                  ^^
  ```

- Warning: `subworkflows/local/quality_control.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/transcript_identification/main.nf:25:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/transcript_identification/main.nf:26:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_identification_bed = Channel.empty()
                              ^^^^^^^
  ```

- Warning: `subworkflows/local/transcript_identification/main.nf:28:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      grohmm_td_plot = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/transcript_identification/main.nf:37:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      homer_peaks = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/transcript_identification/main.nf:38:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      homer_tagdir = Channel.empty()
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/transcript_identification/main.nf:54:21`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { !(it in skip_chr) }
                      ^^
  ```

- Warning: `subworkflows/local/transcript_identification/main.nf:96:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_filter_bed = Channel.from(params.filter_bed)
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/transcript_identification/main.nf:97:113`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          BEDTOOLS_INTERSECT_FILTER(ch_identification_bed.combine(ch_filter_bed.first()), chrom_sizes.map { [[:], it] })
                                                                                                                  ^^
  ```

- Warning: `subworkflows/local/transcript_identification/main.nf:102:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_intersect_bed = Channel.from(params.intersect_bed)
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/transcript_identification/main.nf:103:109`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          BEDTOOLS_INTERSECT(ch_identification_bed.combine(ch_intersect_bed.first()), chrom_sizes.map { [[:], it] })
                                                                                                              ^^
  ```

- Warning: `subworkflows/nf-core/bam_dedup_stats_samtools_umitools/main.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:22:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      bam = bam_bai.map{ [ it[0], it[1] ] }
                           ^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:22:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      bam = bam_bai.map{ [ it[0], it[1] ] }
                                  ^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:24:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:29:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      bamstat_txt = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:40:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      innerdistance_all      = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:41:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      innerdistance_distance = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:42:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      innerdistance_freq     = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:43:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      innerdistance_mean     = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:44:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      innerdistance_pdf      = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:45:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      innerdistance_rscript  = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:61:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      inferexperiment_txt = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:71:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      junctionannotation_all          = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:72:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      junctionannotation_bed          = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:73:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      junctionannotation_interact_bed = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:74:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      junctionannotation_xls          = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:75:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      junctionannotation_pdf          = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:76:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      junctionannotation_events_pdf   = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:77:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      junctionannotation_rscript      = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:78:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      junctionannotation_log          = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:96:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      junctionsaturation_all     = Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:97:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      junctionsaturation_pdf     = Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:98:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      junctionsaturation_rscript = Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:111:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      readdistribution_txt = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:122:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      readduplication_all     = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:123:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      readduplication_seq_xls = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:124:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      readduplication_pos_xls = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:125:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      readduplication_pdf     = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:126:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      readduplication_rscript = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_rseqc/main.nf:141:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tin_txt = Channel.empty()
                ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_sort_stats_samtools/main.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_stats_samtools/main.nf:15:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_align_bowtie2/main.nf:18:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_align_bwa/main.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_align_hisat2/main.nf:14:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_align_star/main.nf:20:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/homer_groseq/main.nf:20:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/homer_groseq/main.nf:22:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_uniqmap = Channel.empty()
                   ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/homer_groseq/main.nf:28:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_uniqmap = UNZIP([[:], uniqmap]).unzipped_archive.map { it[1] }
                                                                    ^^
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

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:72:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/nascent.nf:63:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/nascent.nf:64:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `workflows/nascent.nf:95:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(FASTQC.out.zip.collect { it[1] })
                                                                       ^^
  ```

- Warning: `workflows/nascent.nf:100:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_reads = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `workflows/nascent.nf:113:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_genome_bam = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `workflows/nascent.nf:114:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_genome_bai = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `workflows/nascent.nf:115:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_samtools_stats = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `workflows/nascent.nf:116:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_samtools_flagstat = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `workflows/nascent.nf:117:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_samtools_idxstats = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `workflows/nascent.nf:118:5`: Variable was declared but not used

  ```nextflow
      ch_star_multiqc = Channel.empty()
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/nascent.nf:118:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_star_multiqc = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `workflows/nascent.nf:119:5`: Variable was declared but not used

  ```nextflow
      ch_aligner_pca_multiqc = Channel.empty()
      ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/nascent.nf:119:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_aligner_pca_multiqc = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `workflows/nascent.nf:120:5`: Variable was declared but not used

  ```nextflow
      ch_aligner_clustering_multiqc = Channel.empty()
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/nascent.nf:120:37`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_aligner_clustering_multiqc = Channel.empty()
                                      ^^^^^^^
  ```

- Warning: `workflows/nascent.nf:121:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_bowtie2_multiqc = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `workflows/nascent.nf:206:9`: Variable was declared but not used

  ```nextflow
          ch_HISAT2_multiqc = FASTQ_ALIGN_HISAT2.out.summary
          ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/nascent.nf:213:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  PREPARE_GENOME.out.gtf.map { [[:], it] }
                                                     ^^
  ```

- Warning: `workflows/nascent.nf:228:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              PREPARE_GENOME.out.gtf.map { [[:], it] },
                                                 ^^
  ```

- Warning: `workflows/nascent.nf:233:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              Channel.of([[:], []])
              ^^^^^^^
  ```

- Warning: `workflows/nascent.nf:237:9`: Variable was declared but not used

  ```nextflow
          ch_transcriptome_bam = FASTQ_ALIGN_STAR.out.bam_transcript
          ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/nascent.nf:239:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTQ_ALIGN_STAR.out.stats.collect { it[1] })
                                                                                       ^^
  ```

- Warning: `workflows/nascent.nf:240:89`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTQ_ALIGN_STAR.out.flagstat.collect { it[1] })
                                                                                          ^^
  ```

- Warning: `workflows/nascent.nf:241:89`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTQ_ALIGN_STAR.out.idxstats.collect { it[1] })
                                                                                          ^^
  ```

- Warning: `workflows/nascent.nf:242:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(ch_star_log.collect { it[1] })
                                                                        ^^
  ```

- Warning: `workflows/nascent.nf:280:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def fmeta = meta.findAll { it.key != 'read_group' }
                                         ^^
  ```

- Warning: `workflows/nascent.nf:291:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def fmeta = meta.findAll { it.key != 'read_group' }
                                         ^^
  ```

- Warning: `workflows/nascent.nf:320:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ).saf.map { it[1] }
                          ^^
  ```

- Warning: `workflows/nascent.nf:352:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_workflow_summary = Channel.value(paramsSummaryMultiqc(summary_params))
                            ^^^^^^^
  ```

- Warning: `workflows/nascent.nf:359:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_methods_description = Channel.value(
                               ^^^^^^^
  ```

- Warning: `workflows/nascent.nf:371:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(FASTQC.out.zip.collect { it[1] }.ifEmpty([]))
                                                                       ^^
  ```

- Warning: `workflows/nascent.nf:372:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(ch_bowtie2_multiqc.collect { it[1] }.ifEmpty([]))
                                                                           ^^
  ```

- Warning: `workflows/nascent.nf:373:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(ch_samtools_stats.collect { it[1] }.ifEmpty([]))
                                                                          ^^
  ```

- Warning: `workflows/nascent.nf:374:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(ch_samtools_flagstat.collect { it[1] }.ifEmpty([]))
                                                                             ^^
  ```

- Warning: `workflows/nascent.nf:375:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(ch_samtools_idxstats.collect { it[1] }.ifEmpty([]))
                                                                             ^^
  ```

- Warning: `workflows/nascent.nf:376:89`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(QUALITY_CONTROL.out.preseq_ccurve.collect { it[1] }.ifEmpty([]))
                                                                                          ^^
  ```

- Warning: `workflows/nascent.nf:377:91`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(QUALITY_CONTROL.out.preseq_lcextrap.collect { it[1] }.ifEmpty([]))
                                                                                            ^^
  ```

- Warning: `workflows/nascent.nf:378:96`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(QUALITY_CONTROL.out.readdistribution_txt.collect { it[1] }.ifEmpty([]))
                                                                                                 ^^
  ```

- Warning: `workflows/nascent.nf:379:99`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(QUALITY_CONTROL.out.readduplication_seq_xls.collect { it[1] }.ifEmpty([]))
                                                                                                    ^^
  ```

- Warning: `workflows/nascent.nf:380:99`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(QUALITY_CONTROL.out.readduplication_pos_xls.collect { it[1] }.ifEmpty([]))
                                                                                                    ^^
  ```

- Warning: `workflows/nascent.nf:381:95`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(QUALITY_CONTROL.out.inferexperiment_txt.collect { it[1] }.ifEmpty([]))
                                                                                                ^^
  ```

- Warning: `workflows/nascent.nf:382:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(ch_grohmm_multiqc.collect { it[1] }.ifEmpty([]))
                                                                          ^^
  ```

- Warning: `workflows/nascent.nf:383:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(ch_homer_multiqc.collect { it[1] }.ifEmpty([]))
                                                                         ^^
  ```

- Warning: `workflows/nascent.nf:384:99`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(SUBREAD_FEATURECOUNTS_PREDICTED.out.summary.collect { it[1] }.ifEmpty([]))
                                                                                                    ^^
  ```

- Warning: `workflows/nascent.nf:385:94`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(SUBREAD_FEATURECOUNTS_GENE.out.summary.collect { it[1] }.ifEmpty([]))
                                                                                               ^^
  ```
