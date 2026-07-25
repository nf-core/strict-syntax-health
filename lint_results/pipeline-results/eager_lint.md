# Nextflow lint results

- Generated: 2026-07-25T00:32:14.810999191Z
- Nextflow version: 26.07.0-edge
- Summary: 410 warnings

## :warning: Warnings

- Warning: `modules/local/samtools_view_genome.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/angsd/gl/main.nf:101:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/bcftools/index/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/bcftools/index/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
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

- Warning: `modules/nf-core/circularmapper/circulargenerator/main.nf:50:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/circularmapper/realignsamfile/main.nf:49:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/dedup/main.nf:25:5`: Variable was declared but not used

  ```nextflow
      prefix   = task.ext.prefix ?: "${meta.id}"
      ^^^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:60:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:62:9`: Variable was declared but not used

  ```nextflow
      def paired       = meta.single_end ? "" : "--paired"
          ^^^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:65:9`: Variable was declared but not used

  ```nextflow
      def readclassification_option = save_reads_assignment ? "--output ${prefix}.kraken2.classifiedreads.txt" : "--output /dev/null"
          ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:66:9`: Variable was declared but not used

  ```nextflow
      def compress_reads_command = save_output_fastqs ? "pigz -p $task.cpus *.fastq" : ""
          ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/mapad/index/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/mapdamage2/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/mapdamage2/main.nf:54:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/mtnucratio/main.nf:24:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/samtools/flagstat/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/samtools/idxstats/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/taxpasta/merge/main.nf:31:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/taxpasta/standardise/main.nf:29:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `subworkflows/local/bamfiltering.nf:21:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions       = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/bamfiltering.nf:22:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files  = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/bamfiltering.nf:23:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_flagstats_file = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/bamfiltering.nf:84:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          SAMTOOLS_FASTQ_METAGENOMICS ( bam.map{[ it[0], it[1] ]}, false )
                                                  ^^
  ```

- Warning: `subworkflows/local/bamfiltering.nf:84:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          SAMTOOLS_FASTQ_METAGENOMICS ( bam.map{[ it[0], it[1] ]}, false )
                                                         ^^
  ```

- Warning: `subworkflows/local/bamfiltering.nf:89:100`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_paired_fastq_for_cat_metagenomics = SAMTOOLS_FASTQ_METAGENOMICS.out.fastq.filter { !it[0].single_end }
                                                                                                     ^^
  ```

- Warning: `subworkflows/local/bamfiltering.nf:94:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                          .filter{ it[0].single_end }
                                                   ^^
  ```

- Warning: `subworkflows/local/bamfiltering.nf:103:37`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_fastq_for_metagenomics = Channel.empty()
                                      ^^^^^^^
  ```

- Warning: `subworkflows/local/calculate_damage.nf:17:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions       = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/calculate_damage.nf:18:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files  = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/calculate_damage.nf:24:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              addNewMetaFromAttributes( it, "id" , "reference" , false )
                                        ^^
  ```

- Warning: `subworkflows/local/calculate_damage.nf:30:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              addNewMetaFromAttributes( it, "reference" , "reference" , false )
                                        ^^
  ```

- Warning: `subworkflows/local/calculate_damage.nf:37:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, meta2, fasta_, fasta_fai_ ->
                  ^^^^^^^^^
  ```

- Warning: `subworkflows/local/calculate_damage.nf:37:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, meta2, fasta_, fasta_fai_ ->
                                        ^^^
  ```

- Warning: `subworkflows/local/calculate_damage.nf:37:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, meta2, fasta_, fasta_fai_ ->
                                             ^^^^^
  ```

- Warning: `subworkflows/local/circularmapper.nf:19:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions       = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/circularmapper.nf:20:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files  = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/circularmapper.nf:21:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_realigned_bams = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/circularmapper.nf:22:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_realigned_bais = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/circularmapper.nf:23:5`: Variable was declared but not used

  ```nextflow
      ch_realigned_csis = Channel.empty()
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/circularmapper.nf:23:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_realigned_csis = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/circularmapper.nf:32:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                      meta, index, reference, elongated_chr_list ->
                                            ^^^^^
  ```

- Warning: `subworkflows/local/circularmapper.nf:37:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                      addNewMetaFromAttributes( it, "id" , "reference" , false )
                                                                ^^
  ```

- Warning: `subworkflows/local/circularmapper.nf:49:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                      addNewMetaFromAttributes( it, "reference" , "reference" , false )
                                                                ^^
  ```

- Warning: `subworkflows/local/circularmapper.nf:53:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                      ignore_me, meta, bam, ref_meta, ref_fasta, elongated_chr_list ->
                                      ^^^^^^^^^
  ```

- Warning: `subworkflows/local/consensus_sequence.nf:18:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/consensus_sequence.nf:19:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/consensus_sequence.nf:24:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, vcfs, vcf_index ->
                              ^^^^^^^^^
  ```

- Warning: `subworkflows/local/consensus_sequence.nf:28:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes(it, "reference", "reference", true)
                                           ^^
  ```

- Warning: `subworkflows/local/consensus_sequence.nf:34:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          addNewMetaFromAttributes(it, "vcf_reference_id", "reference", true)
                                                   ^^
  ```

- Warning: `subworkflows/local/consensus_sequence.nf:39:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  merge_meta, vcfs ->
                  ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/consensus_sequence.nf:46:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes(it, "id", "reference", true)
                                           ^^
  ```

- Warning: `subworkflows/local/consensus_sequence.nf:48:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, fasta, fai, dict, mapindex ->
                                  ^^^
  ```

- Warning: `subworkflows/local/consensus_sequence.nf:48:38`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, fasta, fai, dict, mapindex ->
                                       ^^^^
  ```

- Warning: `subworkflows/local/consensus_sequence.nf:48:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, fasta, fai, dict, mapindex ->
                                             ^^^^^^^^
  ```

- Warning: `subworkflows/local/consensus_sequence.nf:54:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes(it, "id", "reference", true)
                                           ^^
  ```

- Warning: `subworkflows/local/deduplicate.nf:23:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/deduplicate.nf:24:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files  = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/deduplicate.nf:29:35`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          addNewMetaFromAttributes( it, "id" , "reference" , false )
                                    ^^
  ```

- Warning: `subworkflows/local/deduplicate.nf:47:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              addNewMetaFromAttributes( it, "id" , "reference" , true )
                                        ^^
  ```

- Warning: `subworkflows/local/deduplicate.nf:54:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes( it, "reference" , "reference" , false )
                                            ^^
  ```

- Warning: `subworkflows/local/deduplicate.nf:61:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, regions ->
                  ^^^^^^^^^
  ```

- Warning: `subworkflows/local/deduplicate.nf:77:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes( it, "reference" , "reference" , false )
                                            ^^
  ```

- Warning: `subworkflows/local/deduplicate.nf:84:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, meta2, fasta_, fasta_fai_ ->
                  ^^^^^^^^^
  ```

- Warning: `subworkflows/local/deduplicate.nf:84:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, meta2, fasta_, fasta_fai_ ->
                                        ^^^
  ```

- Warning: `subworkflows/local/deduplicate.nf:103:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, bam, bai ->
                             ^^^
  ```

- Warning: `subworkflows/local/deduplicate.nf:124:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def meta2 = meta.clone().findAll{ it.key != 'genomic_region' }
                                                    ^^
  ```

- Warning: `subworkflows/local/deduplicate.nf:130:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes( it, "reference" , "reference" , false )
                                            ^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:16:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions           = Channel.empty()
                              ^^^^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:17:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files      = Channel.empty()
                              ^^^^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:18:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_circular_reference = Channel.empty()
                              ^^^^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:19:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_elongated_unzipped = Channel.empty()
                              ^^^^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:20:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_elongated_chr      = Channel.empty()
                              ^^^^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:25:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, circular_target, circularmapper_elongated_fasta, circularmapper_elongated_index ->
                                  ^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:25:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, circular_target, circularmapper_elongated_fasta, circularmapper_elongated_index ->
                                        ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:25:88`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, circular_target, circularmapper_elongated_fasta, circularmapper_elongated_index ->
                                                                                         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:32:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, circular_target, circularmapper_elongated_fasta, circularmapper_elongated_index ->
                                        ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:32:88`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, circular_target, circularmapper_elongated_fasta, circularmapper_elongated_index ->
                                                                                         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:43:41`: Variable was declared but not used

  ```nextflow
                                      def final_fasta = unzipped_fasta ?: circularmapper_elongated_fasta
                                          ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:59:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, circular_target, circularmapper_elongated_fasta, circularmapper_elongated_index ->
                                  ^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:75:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                  addNewMetaFromAttributes( it, "id", "id", false )
                                                            ^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:82:56`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, circular_target, circularmapper_elongated_fasta, circularmapper_elongated_index, fasta, fai, dict, mapindex ->
                                                         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:82:88`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, circular_target, circularmapper_elongated_fasta, circularmapper_elongated_index, fasta, fai, dict, mapindex ->
                                                                                         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:82:127`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, circular_target, circularmapper_elongated_fasta, circularmapper_elongated_index, fasta, fai, dict, mapindex ->
                                                                                                                                ^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:82:132`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, circular_target, circularmapper_elongated_fasta, circularmapper_elongated_index, fasta, fai, dict, mapindex ->
                                                                                                                                     ^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:82:138`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, circular_target, circularmapper_elongated_fasta, circularmapper_elongated_index, fasta, fai, dict, mapindex ->
                                                                                                                                           ^^^^^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:86:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, fasta, circular_target ->
                                  ^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:96:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  ignore_me, chr_list, meta, fasta, fai, dict, mapindex ->
                                  ^^^^^^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:96:60`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  ignore_me, chr_list, meta, fasta, fai, dict, mapindex ->
                                                             ^^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:96:67`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  ignore_me, chr_list, meta, fasta, fai, dict, mapindex ->
                                                                    ^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:96:72`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  ignore_me, chr_list, meta, fasta, fai, dict, mapindex ->
                                                                         ^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:96:78`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  ignore_me, chr_list, meta, fasta, fai, dict, mapindex ->
                                                                               ^^^^^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:105:56`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, circular_target, circularmapper_elongated_fasta, circularmapper_elongated_index, fasta, fai, dict, mapindex ->
                                                         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:105:88`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, circular_target, circularmapper_elongated_fasta, circularmapper_elongated_index, fasta, fai, dict, mapindex ->
                                                                                         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:105:127`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, circular_target, circularmapper_elongated_fasta, circularmapper_elongated_index, fasta, fai, dict, mapindex ->
                                                                                                                                ^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:105:132`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, circular_target, circularmapper_elongated_fasta, circularmapper_elongated_index, fasta, fai, dict, mapindex ->
                                                                                                                                     ^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:105:138`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, circular_target, circularmapper_elongated_fasta, circularmapper_elongated_index, fasta, fai, dict, mapindex ->
                                                                                                                                           ^^^^^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:125:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, circular_target, circularmapper_elongated_fasta, circularmapper_elongated_index ->
                                        ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:125:88`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, circular_target, circularmapper_elongated_fasta, circularmapper_elongated_index ->
                                                                                         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/elongate_reference.nf:139:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, circular_target, circularmapper_elongated_fasta, circularmapper_elongated_index ->
                                        ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/estimate_contamination.nf:17:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions       = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/estimate_contamination.nf:18:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files  = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/estimate_contamination.nf:24:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes( it, "id" , "reference" , false )
                                            ^^
  ```

- Warning: `subworkflows/local/estimate_contamination.nf:29:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes( it, "reference" , "reference" , false )
                                            ^^
  ```

- Warning: `subworkflows/local/estimate_contamination.nf:36:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, meta2, hapmap ->
                  ^^^^^^^^^
  ```

- Warning: `subworkflows/local/estimate_contamination.nf:36:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, meta2, hapmap ->
                                             ^^^^^
  ```

- Warning: `subworkflows/local/estimate_contamination.nf:46:35`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                              .map{ it[1] } //remove meta
                                    ^^
  ```

- Warning: `subworkflows/local/genotype.nf:28:42`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions                        = Channel.empty()
                                           ^^^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:29:42`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files                   = Channel.empty()
                                           ^^^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:30:42`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_pileupcaller_genotypes          = Channel.empty()
                                           ^^^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:31:42`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_eigenstrat_coverage_stats       = Channel.empty()
                                           ^^^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:32:42`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_angsd_genotype_likelihoods      = Channel.empty()
                                           ^^^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:33:42`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_genotypes_vcf                   = Channel.empty()
                                           ^^^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:34:42`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_bcftools_stats                  = Channel.empty()
                                           ^^^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:43:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter { it[0] != [] }
                        ^^
  ```

- Warning: `subworkflows/local/genotype.nf:54:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ref_meta, fasta, fai, dict, empty ->
                                              ^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:60:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes( it, "id" , "reference" , false )
                                            ^^
  ```

- Warning: `subworkflows/local/genotype.nf:66:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes( it, ["reference", "strandedness"] , ["reference", "strandedness"] , false )
                                            ^^
  ```

- Warning: `subworkflows/local/genotype.nf:70:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  combo_meta, metas, bams, bais ->
                                           ^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:78:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      addNewMetaFromAttributes( it, "reference", "reference" , false )
                                                ^^
  ```

- Warning: `subworkflows/local/genotype.nf:82:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .filter { it[7] != []}
                            ^^
  ```

- Warning: `subworkflows/local/genotype.nf:84:21`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      ignore_me, combo_meta, bams, ref_meta, fasta, fai, dict, bed, snp ->
                      ^^^^^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:84:67`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      ignore_me, combo_meta, bams, ref_meta, fasta, fai, dict, bed, snp ->
                                                                    ^^^
  ```

- Warning: `subworkflows/local/genotype.nf:84:72`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      ignore_me, combo_meta, bams, ref_meta, fasta, fai, dict, bed, snp ->
                                                                         ^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:84:83`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      ignore_me, combo_meta, bams, ref_meta, fasta, fai, dict, bed, snp ->
                                                                                    ^^^
  ```

- Warning: `subworkflows/local/genotype.nf:98:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      addNewMetaFromAttributes( it, "reference", "reference" , false )
                                                ^^
  ```

- Warning: `subworkflows/local/genotype.nf:102:21`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      ignore_me, meta, mpileup, ref_meta, fasta, fai, dict, bed, snp ->
                      ^^^^^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:102:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      ignore_me, meta, mpileup, ref_meta, fasta, fai, dict, bed, snp ->
                                                ^^^^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:102:57`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      ignore_me, meta, mpileup, ref_meta, fasta, fai, dict, bed, snp ->
                                                          ^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:102:64`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      ignore_me, meta, mpileup, ref_meta, fasta, fai, dict, bed, snp ->
                                                                 ^^^
  ```

- Warning: `subworkflows/local/genotype.nf:102:69`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      ignore_me, meta, mpileup, ref_meta, fasta, fai, dict, bed, snp ->
                                                                      ^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:102:75`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      ignore_me, meta, mpileup, ref_meta, fasta, fai, dict, bed, snp ->
                                                                            ^^^
  ```

- Warning: `subworkflows/local/genotype.nf:119:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      addNewMetaFromAttributes( it, "reference" , "reference" , false )
                                                ^^
  ```

- Warning: `subworkflows/local/genotype.nf:123:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      combo_meta, metas, geno, snp, ind ->
                                  ^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:150:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes( it, "reference" , "reference" , false )
                                            ^^
  ```

- Warning: `subworkflows/local/genotype.nf:157:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter { it[0] != [] }
                        ^^
  ```

- Warning: `subworkflows/local/genotype.nf:166:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes( it, "id" , "reference" , false )
                                            ^^
  ```

- Warning: `subworkflows/local/genotype.nf:172:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta, fai, dict, dbsnp ->
                  ^^^^^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:172:72`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta, fai, dict, dbsnp ->
                                                                         ^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:193:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes( it, "reference" , "reference" , false )
                                            ^^
  ```

- Warning: `subworkflows/local/genotype.nf:197:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, intervals, ref_meta, fasta, fai, dict, dbsnp ->
                  ^^^^^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:197:83`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, intervals, ref_meta, fasta, fai, dict, dbsnp ->
                                                                                    ^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:216:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes( it, "reference" , "reference" , false )
                                            ^^
  ```

- Warning: `subworkflows/local/genotype.nf:220:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta, fai, dict, dbsnp ->
                  ^^^^^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:257:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes( it, "reference" , "reference" , false )
                                            ^^
  ```

- Warning: `subworkflows/local/genotype.nf:264:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter { it[0] != [] }
                        ^^
  ```

- Warning: `subworkflows/local/genotype.nf:273:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes( it, "id" , "reference" , false )
                                            ^^
  ```

- Warning: `subworkflows/local/genotype.nf:279:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta, fai, dict, dbsnp ->
                  ^^^^^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:308:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes( it, "reference" , "reference" , false )
                                            ^^
  ```

- Warning: `subworkflows/local/genotype.nf:317:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter { it[0] != [] }
                        ^^
  ```

- Warning: `subworkflows/local/genotype.nf:326:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes( it, "id" , "reference" , false )
                                            ^^
  ```

- Warning: `subworkflows/local/genotype.nf:332:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta, fai, dict, dbsnp ->
                  ^^^^^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:332:66`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta, fai, dict, dbsnp ->
                                                                   ^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:332:72`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta, fai, dict, dbsnp ->
                                                                         ^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:365:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes( it, "reference" , "reference" , false )
                                            ^^
  ```

- Warning: `subworkflows/local/genotype.nf:370:25`: Variable was declared but not used

  ```nextflow
                      def new_map = [:]
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:384:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter { it[0] != [] }
                        ^^
  ```

- Warning: `subworkflows/local/genotype.nf:393:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes( it, "id" , "reference" , false )
                                            ^^
  ```

- Warning: `subworkflows/local/genotype.nf:400:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta, fai, dict, dbsnp ->
                  ^^^^^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:400:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta, fai, dict, dbsnp ->
                                        ^^^
  ```

- Warning: `subworkflows/local/genotype.nf:400:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta, fai, dict, dbsnp ->
                                             ^^^^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:400:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta, fai, dict, dbsnp ->
                                                       ^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:400:61`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta, fai, dict, dbsnp ->
                                                              ^^^
  ```

- Warning: `subworkflows/local/genotype.nf:400:66`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta, fai, dict, dbsnp ->
                                                                   ^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:400:72`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta, fai, dict, dbsnp ->
                                                                         ^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:424:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes( it, "reference" , "reference" , false )
                                            ^^
  ```

- Warning: `subworkflows/local/genotype.nf:428:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, vcf, tbi, ref_meta, fasta, fai, dict, dbsnp ->
                  ^^^^^^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:428:61`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, vcf, tbi, ref_meta, fasta, fai, dict, dbsnp ->
                                                              ^^^
  ```

- Warning: `subworkflows/local/genotype.nf:428:66`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, vcf, tbi, ref_meta, fasta, fai, dict, dbsnp ->
                                                                   ^^^^
  ```

- Warning: `subworkflows/local/genotype.nf:428:72`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, vcf, tbi, ref_meta, fasta, fai, dict, dbsnp ->
                                                                         ^^^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:24:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions              = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:25:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_rescaled_bams         = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:26:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_pmd_filtered_bams     = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:27:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_trimmed_bams          = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:28:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_pmd_filtered_flagstat = Channel.empty() // Only run flagstat on pmd filtered bam, since rescaling and trimming does not change the number of reads
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:34:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              addNewMetaFromAttributes( it, "id" , "reference" , false )
                                        ^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:40:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              addNewMetaFromAttributes( it, "reference" , "reference" , false )
                                        ^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:47:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta ->
                  ^^^^^^^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:47:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta ->
                                   ^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:47:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta ->
                                        ^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:47:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta ->
                                             ^^^^^^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:47:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta ->
                                                       ^^^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:54:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta ->
                  ^^^^^^^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:54:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta ->
                                             ^^^^^^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:54:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta ->
                                                       ^^^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:60:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta ->
                  ^^^^^^^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:60:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta ->
                                        ^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:60:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ignore_me, meta, bam, bai, ref_meta, fasta ->
                                             ^^^^^^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:81:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          meta, masked_fasta, bed, fasta ->
                          ^^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:81:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          meta, masked_fasta, bed, fasta ->
                                                   ^^^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:89:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          meta, masked_fasta, bed, fasta ->
                                ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:100:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          meta, masked_fasta, bed, fasta ->
                                              ^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:100:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          meta, masked_fasta, bed, fasta ->
                                                   ^^^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:106:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          meta, masked_fasta, bed, fasta ->
                                ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:106:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          meta, masked_fasta, bed, fasta ->
                                              ^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:113:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          addNewMetaFromAttributes( it, "id" , "reference" , false )
                                                    ^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:117:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .map { addNewMetaFromAttributes( it, "reference" , "reference" , false ) }
                                                       ^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:120:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          combine_meta, meta, bam, bai, ref_meta, fasta ->
                          ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:120:55`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          combine_meta, meta, bam, bai, ref_meta, fasta ->
                                                        ^^^^^^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:143:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      meta, bam, bai ->
                                 ^^^
  ```

- Warning: `subworkflows/local/manipulate_damage.nf:149:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      meta, bam, bai ->
                                 ^^^
  ```

- Warning: `subworkflows/local/map.nf:28:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions       = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/map.nf:29:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files  = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/map.nf:55:57`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_index_for_mapping = index.map{ meta, index_, fasta -> [ meta, index_ ] }
                                                          ^^^^^
  ```

- Warning: `subworkflows/local/map.nf:91:64`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              .combine( index.map{ meta, index_, fasta -> [ meta, index_ ] } )
                                                                 ^^^^^
  ```

- Warning: `subworkflows/local/map.nf:110:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, elongated_fasta, elongated_index ->
                                        ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/map.nf:120:64`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              .combine( index.map{ meta, index_, fasta -> [ meta, index_ ] } )
                                                                 ^^^^^
  ```

- Warning: `subworkflows/local/map.nf:162:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                      def new_meta = meta.clone().findAll{ it.key !in ['lane', 'colour_chemistry', 'shard_number'] }
                                                                           ^^
  ```

- Warning: `subworkflows/local/map.nf:167:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                      meta, bam ->
                                      ^^^^
  ```

- Warning: `subworkflows/local/merge_lanes_inputbam.nf:15:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions       = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/merge_lanes_inputbam.nf:16:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files  = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/merge_lanes_inputbam.nf:19:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                  .map { meta, bam -> [ meta.clone().findAll{ it.key !in ['lane', 'colour_chemistry', 'shard_number'] }, bam ] }
                                                                              ^^
  ```

- Warning: `subworkflows/local/merge_lanes_inputbam.nf:22:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                      meta, bam ->
                                      ^^^^
  ```

- Warning: `subworkflows/local/merge_libraries.nf:17:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions      = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/merge_libraries.nf:18:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/merge_libraries.nf:21:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { addNewMetaFromAttributes( it, ["id", "sample_id", "strandedness", "reference"], ["id", "sample_id", "strandedness", "reference"], false ) }
                                           ^^
  ```

- Warning: `subworkflows/local/merge_libraries.nf:25:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, lib_metas, bam, bai ->
                    ^^^^^^^^^
  ```

- Warning: `subworkflows/local/merge_libraries.nf:25:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, lib_metas, bam, bai ->
                                    ^^^
  ```

- Warning: `subworkflows/local/metagenomics.nf:14:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files                = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/local/metagenomics.nf:15:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions                     = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/local/metagenomics.nf:30:97`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(METAGENOMICS_COMPLEXITYFILTER.out.fastq.collect{it[1]}.ifEmpty([]))
                                                                                                  ^^
  ```

- Warning: `subworkflows/local/metagenomics.nf:41:85`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix( METAGENOMICS_PROFILING.out.mqc.collect{it[1]}.ifEmpty([]) )
                                                                                      ^^
  ```

- Warning: `subworkflows/local/metagenomics.nf:52:94`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix( METAGENOMICS_POSTPROCESSING.out.mqc.collect{it[1]}.ifEmpty([]) )
                                                                                               ^^
  ```

- Warning: `subworkflows/local/metagenomics_postprocessing.nf:15:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions      = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/metagenomics_postprocessing.nf:16:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/metagenomics_postprocessing.nf:38:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  rma6:[it[0],it[1]]
                        ^^
  ```

- Warning: `subworkflows/local/metagenomics_postprocessing.nf:38:29`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  rma6:[it[0],it[1]]
                              ^^
  ```

- Warning: `subworkflows/local/metagenomics_postprocessing.nf:39:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  tax_list:it[2]
                           ^^
  ```

- Warning: `subworkflows/local/metagenomics_postprocessing.nf:40:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ncbi_dir:it[3]
                           ^^
  ```

- Warning: `subworkflows/local/metagenomics_postprocessing.nf:47:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_amps_input = MALTEXTRACT.out.results.map{ it[1] }
                                                       ^^
  ```

- Warning: `subworkflows/local/metagenomics_postprocessing.nf:79:13`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, report ->
              ^^^^
  ```

- Warning: `subworkflows/local/metagenomics_postprocessing.nf:91:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              standardise: it[2] == 1
                           ^^
  ```

- Warning: `subworkflows/local/metagenomics_postprocessing.nf:95:84`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_standardise_input = ch_postprocessing_input.standardise.map{ meta, reports, count ->
                                                                                     ^^^^^
  ```

- Warning: `subworkflows/local/metagenomics_postprocessing.nf:102:72`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_merge_input = ch_postprocessing_input.merge.map{ meta, reports, count ->
                                                                         ^^^^^
  ```

- Warning: `subworkflows/local/metagenomics_profiling.nf:21:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions             = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/metagenomics_profiling.nf:22:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files        = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/metagenomics_profiling.nf:23:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_postprocessing_input = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/metagenomics_profiling.nf:31:16`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          untar: it ==~ /.*.tar.gz/
                 ^^
  ```

- Warning: `subworkflows/local/metagenomics_profiling.nf:36:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_untar_input = ch_database.untar.map{ [[], it] }
                                                   ^^
  ```

- Warning: `subworkflows/local/metagenomics_profiling.nf:39:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_untar_output = UNTAR_METAGENOMICS.out.untar.map{ it[1] }
                                                          ^^
  ```

- Warning: `subworkflows/local/metagenomics_profiling.nf:69:132`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_tmp_groups =  params.metagenomics_malt_group_size > 0 ? ch_reads.collate(params.metagenomics_malt_group_size).count() : Channel.of(1)
                                                                                                                                     ^^^^^^^
  ```

- Warning: `subworkflows/local/metagenomics_profiling.nf:112:21`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      meta,log -> log
                      ^^^^
  ```

- Warning: `subworkflows/local/preprocessing.nf:17:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions       = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/preprocessing.nf:18:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files  = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/preprocessing_adapterremoval.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/preprocessing_adapterremoval.nf:17:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files      = Channel.empty()
                              ^^^^^^^
  ```

- Warning: `subworkflows/local/preprocessing_adapterremoval.nf:21:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                          single: it[0].single_end
                                                  ^^
  ```

- Warning: `subworkflows/local/preprocessing_adapterremoval.nf:22:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                                          paired: !it[0].single_end
                                                   ^^
  ```

- Warning: `subworkflows/local/preprocessing_adapterremoval.nf:41:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_concat_fastq = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/preprocessing_adapterremoval.nf:67:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_concat_fastq = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/preprocessing_fastp.nf:14:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/preprocessing_fastp.nf:15:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/preprocessing_fastp.nf:18:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          single: it[0]['single_end'] == true
                  ^^
  ```

- Warning: `subworkflows/local/preprocessing_fastp.nf:19:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          paired: it[0]['single_end'] == false
                  ^^
  ```

- Warning: `subworkflows/local/reference_indexing.nf:20:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/reference_indexing.nf:62:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .filter{ it[1] != "" }
                               ^^
  ```

- Warning: `subworkflows/local/reference_indexing.nf:65:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .filter{ it[1] != "" }
                               ^^
  ```

- Warning: `subworkflows/local/reference_indexing.nf:69:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          meta, pmd_masked_fasta ->
                          ^^^^
  ```

- Warning: `subworkflows/local/reference_indexing.nf:75:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          meta, pmd_masked_fasta ->
                          ^^^^
  ```

- Warning: `subworkflows/local/reference_indexing.nf:85:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          meta, pmd_bed_for_masking ->
                          ^^^^
  ```

- Warning: `subworkflows/local/reference_indexing.nf:91:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          meta, pmd_bed_for_masking ->
                          ^^^^
  ```

- Warning: `subworkflows/local/reference_indexing.nf:104:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          meta, capture_bed ->
                          ^^^^
  ```

- Warning: `subworkflows/local/reference_indexing.nf:110:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          meta, capture_bed ->
                          ^^^^
  ```

- Warning: `subworkflows/local/reference_indexing.nf:119:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .filter { it[1] != "" || it[2] != "" } // They go together or not at all.
                                ^^
  ```

- Warning: `subworkflows/local/reference_indexing.nf:119:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .filter { it[1] != "" || it[2] != "" } // They go together or not at all.
                                               ^^
  ```

- Warning: `subworkflows/local/reference_indexing.nf:122:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .filter{ it != null } // Remove null channel which arises if empty cause error returns null.
                               ^^
  ```

- Warning: `subworkflows/local/reference_indexing.nf:125:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .filter { it[1] != "" }
                                ^^
  ```

- Warning: `subworkflows/local/reference_indexing.nf:128:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .filter { it[1] != "" }
                                ^^
  ```

- Warning: `subworkflows/local/reference_indexing.nf:131:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it[1] != "" }
                    ^^
  ```

- Warning: `subworkflows/local/reference_indexing.nf:137:9`: Variable was declared but not used

  ```nextflow
          ch_elongated_for_gunzip = ch_reference_to_elongate
          ^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/reference_indexing.nf:139:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              meta, circular_target, circularmapper_elongatedfasta, circularmapper_elongatedindex ->
                              ^^^^
  ```

- Warning: `subworkflows/local/reference_indexing.nf:139:52`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              meta, circular_target, circularmapper_elongatedfasta, circularmapper_elongatedindex ->
                                                     ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/reference_indexing.nf:139:83`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              meta, circular_target, circularmapper_elongatedfasta, circularmapper_elongatedindex ->
                                                                                    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/reference_indexing.nf:152:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_elongated_chr_list = Channel.empty()
                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_multi.nf:18:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_multi.nf:21:41`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_splitreferencesheet_for_branch = Channel
                                          ^^^^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_multi.nf:74:75`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta_for_gunzip = ch_input_from_referencesheet.generated.branch { meta, fasta, fai, dict, mapper_index ->
                                                                            ^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_multi.nf:74:88`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta_for_gunzip = ch_input_from_referencesheet.generated.branch { meta, fasta, fai, dict, mapper_index ->
                                                                                         ^^^
  ```

- Warning: `subworkflows/local/reference_indexing_multi.nf:74:93`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta_for_gunzip = ch_input_from_referencesheet.generated.branch { meta, fasta, fai, dict, mapper_index ->
                                                                                              ^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_multi.nf:74:99`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta_for_gunzip = ch_input_from_referencesheet.generated.branch { meta, fasta, fai, dict, mapper_index ->
                                                                                                    ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_multi.nf:98:60`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta_for_faidx = ch_fasta_for_faiindexing.branch { meta, fasta, fai, dict, mapper_index ->
                                                             ^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_multi.nf:98:66`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta_for_faidx = ch_fasta_for_faiindexing.branch { meta, fasta, fai, dict, mapper_index ->
                                                                   ^^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_multi.nf:98:78`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta_for_faidx = ch_fasta_for_faiindexing.branch { meta, fasta, fai, dict, mapper_index ->
                                                                               ^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_multi.nf:98:84`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta_for_faidx = ch_fasta_for_faiindexing.branch { meta, fasta, fai, dict, mapper_index ->
                                                                                     ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_multi.nf:104:74`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_faidx_input = ch_fasta_for_faidx.forfaidx.multiMap { meta, fasta, fai, dict, mapper_index ->
                                                                           ^^^
  ```

- Warning: `subworkflows/local/reference_indexing_multi.nf:127:60`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta_for_dict = ch_fasta_for_dictindexing.branch { meta, fasta, fai, dict, mapper_index ->
                                                             ^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_multi.nf:127:66`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta_for_dict = ch_fasta_for_dictindexing.branch { meta, fasta, fai, dict, mapper_index ->
                                                                   ^^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_multi.nf:127:73`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta_for_dict = ch_fasta_for_dictindexing.branch { meta, fasta, fai, dict, mapper_index ->
                                                                          ^^^
  ```

- Warning: `subworkflows/local/reference_indexing_multi.nf:127:84`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta_for_dict = ch_fasta_for_dictindexing.branch { meta, fasta, fai, dict, mapper_index ->
                                                                                     ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_multi.nf:132:76`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_dict_input = ch_fasta_for_dict.fordict.multiMap { meta, fasta, fai, dict, mapper_index ->
                                                                             ^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_multi.nf:155:67`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta_for_mapperindex = ch_dict_formapperindexing.branch { meta, fasta, fai, dict, mapper_index ->
                                                                    ^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_multi.nf:155:73`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta_for_mapperindex = ch_dict_formapperindexing.branch { meta, fasta, fai, dict, mapper_index ->
                                                                          ^^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_multi.nf:155:80`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta_for_mapperindex = ch_dict_formapperindexing.branch { meta, fasta, fai, dict, mapper_index ->
                                                                                 ^^^
  ```

- Warning: `subworkflows/local/reference_indexing_multi.nf:155:85`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta_for_mapperindex = ch_dict_formapperindexing.branch { meta, fasta, fai, dict, mapper_index ->
                                                                                      ^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_multi.nf:160:94`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_mapindex_input = ch_fasta_for_mapperindex.forindex.multiMap { meta, fasta, fai, dict, mapper_index ->
                                                                                               ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_single.nf:23:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_single.nf:30:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gz_ref = Channel.fromPath(fasta).map{[[], it]}
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_single.nf:30:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_gz_ref = Channel.fromPath(fasta).map{[[], it]}
                                                       ^^
  ```

- Warning: `subworkflows/local/reference_indexing_single.nf:32:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_ungz_ref = GUNZIP_FASTA.out.gunzip.map{[[id: clean_name], it[1] ]}
                                                                       ^^
  ```

- Warning: `subworkflows/local/reference_indexing_single.nf:35:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_ungz_ref = Channel.fromPath(fasta).map{[[id: clean_name], it ]}
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_single.nf:35:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_ungz_ref = Channel.fromPath(fasta).map{[[id: clean_name], it ]}
                                                                       ^^
  ```

- Warning: `subworkflows/local/reference_indexing_single.nf:40:104`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta_fai = SAMTOOLS_FAIDX ( ch_ungz_ref, [ [], [] ] ).fai.map{[ [id: clean_name - '.fai'], it[1] ] }
                                                                                                         ^^
  ```

- Warning: `subworkflows/local/reference_indexing_single.nf:43:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_fasta_fai = Channel.fromPath(fasta_fai).map{[[id: clean_name], it ]}
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_single.nf:43:75`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta_fai = Channel.fromPath(fasta_fai).map{[[id: clean_name], it ]}
                                                                            ^^
  ```

- Warning: `subworkflows/local/reference_indexing_single.nf:48:121`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta_dict = PICARD_CREATESEQUENCEDICTIONARY ( ch_ungz_ref ).reference_dict.map{[ [id: clean_name - '.fai'], it[1] ] }
                                                                                                                          ^^
  ```

- Warning: `subworkflows/local/reference_indexing_single.nf:51:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_fasta_dict = Channel.fromPath(fasta_dict).map{[[id: clean_name], it ]}
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_single.nf:51:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta_dict = Channel.fromPath(fasta_dict).map{[[id: clean_name], it ]}
                                                                              ^^
  ```

- Warning: `subworkflows/local/reference_indexing_single.nf:61:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_fasta_mapperindexdir = Channel.fromPath(fasta_mapperindexdir).map{[[id: clean_name], it ]}
                                        ^^^^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_single.nf:61:101`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_fasta_mapperindexdir = Channel.fromPath(fasta_mapperindexdir).map{[[id: clean_name], it ]}
                                                                                                      ^^
  ```

- Warning: `subworkflows/local/reference_indexing_single.nf:70:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_fasta_mapperindexdir = Channel.fromPath(fasta_mapperindexdir).map{[[id: clean_name], it ]}
                                        ^^^^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_single.nf:70:101`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_fasta_mapperindexdir = Channel.fromPath(fasta_mapperindexdir).map{[[id: clean_name], it ]}
                                                                                                      ^^
  ```

- Warning: `subworkflows/local/reference_indexing_single.nf:79:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_fasta_mapperindexdir = Channel.fromPath(fasta_mapperindexdir).map{[[id: clean_name], it ]}
                                        ^^^^^^^
  ```

- Warning: `subworkflows/local/reference_indexing_single.nf:79:101`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_fasta_mapperindexdir = Channel.fromPath(fasta_mapperindexdir).map{[[id: clean_name], it ]}
                                                                                                      ^^
  ```

- Warning: `subworkflows/local/run_sex_determination.nf:17:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions       = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/run_sex_determination.nf:18:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files  = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/run_sex_determination.nf:27:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes( it, "id" , "reference" , false )
                                            ^^
  ```

- Warning: `subworkflows/local/run_sex_determination.nf:33:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes( it, "reference" , "reference" , false )
                                            ^^
  ```

- Warning: `subworkflows/local/run_sex_determination.nf:38:41`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  combo_meta, metas, bam, bai, ref_meta, bed ->
                                          ^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_eager_pipeline/main.nf:120:41`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                          meta, r1, r2, bam, vcf ->
                                          ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_eager_pipeline/main.nf:120:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                          meta, r1, r2, bam, vcf ->
                                                ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_eager_pipeline/main.nf:120:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                          meta, r1, r2, bam, vcf ->
                                                    ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_eager_pipeline/main.nf:128:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                      meta, r1, r2, bam, vcf ->
                                                    ^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_eager_pipeline/main.nf:128:56`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                      meta, r1, r2, bam, vcf ->
                                                         ^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_eager_pipeline/main.nf:135:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, r1, r2, bam, vcf ->
                                        ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_eager_pipeline/main.nf:135:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, r1, r2, bam, vcf ->
                                            ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_eager_pipeline/main.nf:135:52`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, r1, r2, bam, vcf ->
                                                     ^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_eager_pipeline/main.nf:143:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, r1, r2, bam, vcf ->
                                        ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_eager_pipeline/main.nf:143:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, r1, r2, bam, vcf ->
                                            ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_eager_pipeline/main.nf:143:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, r1, r2, bam, vcf ->
                                                ^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_eager_pipeline/main.nf:188:5`: Variable was declared but not used

  ```nextflow
      ch_samplesheet_test = ch_samplesheet
      ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_eager_pipeline/main.nf:190:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, r1, r2, bam, vcf ->
                                        ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_eager_pipeline/main.nf:190:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, r1, r2, bam, vcf ->
                                            ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_eager_pipeline/main.nf:190:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, r1, r2, bam, vcf ->
                                                ^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_eager_pipeline/main.nf:190:52`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  meta, r1, r2, bam, vcf ->
                                                     ^^^
  ```

- Warning: `subworkflows/nf-core/bam_docounts_contamination_angsd/main.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_split_by_region/main.nf:15:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_split_by_region/main.nf:23:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, bam, bai, regions_file ->
                    ^^^
  ```

- Warning: `subworkflows/nf-core/bam_split_by_region/main.nf:23:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, bam, bai, regions_file ->
                         ^^^
  ```

- Warning: `subworkflows/nf-core/bam_split_by_region/main.nf:50:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta, bam, bai, regions, chrom -> [ meta + [ genomic_region:chrom ], bam, bai ] }
                                ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_align_bwaaln/main.nf:18:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_align_bwaaln/main.nf:45:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              meta, reads, meta_index, index ->
                                           ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_align_bwaaln/main.nf:53:57`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_reads_newid = ch_prepped_input.map{ meta, reads, meta_index, index -> [ meta, reads ] }
                                                          ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_align_bwaaln/main.nf:53:69`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_reads_newid = ch_prepped_input.map{ meta, reads, meta_index, index -> [ meta, reads ] }
                                                                      ^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_align_bwaaln/main.nf:54:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_index_newid = ch_prepped_input.map{ meta, reads, meta_index, index -> [ meta, index ] }
                                                   ^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_align_bwaaln/main.nf:54:57`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_index_newid = ch_prepped_input.map{ meta, reads, meta_index, index -> [ meta, index ] }
                                                          ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_align_bwaaln/main.nf:63:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              meta, reads, sai ->
                                    ^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_align_bwaaln/main.nf:63:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              meta, reads, sai ->
                                           ^^^
  ```

- Warning: `workflows/eager.nf:118:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, reads ->
                              ^^^^^
  ```

- Warning: `workflows/eager.nf:130:83`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_paired_end_reads = SAMTOOLS_CONVERT_BAM_INPUT.out.fastq.filter { meta, reads ->
                                                                                    ^^^^^
  ```

- Warning: `workflows/eager.nf:164:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FALCO.out.txt.collect { it[1] }.ifEmpty([]))
                                                                          ^^
  ```

- Warning: `workflows/eager.nf:169:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTQC.out.zip.collect { it[1] }.ifEmpty([]))
                                                                           ^^
  ```

- Warning: `workflows/eager.nf:180:81`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(PREPROCESSING.out.mqc.collect { it[1] }.ifEmpty([]))
                                                                                  ^^
  ```

- Warning: `workflows/eager.nf:189:84`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_reference_for_mapping = REFERENCE_INDEXING.out.reference.map { meta, fasta, fai, dict, index ->
                                                                                     ^^^
  ```

- Warning: `workflows/eager.nf:189:89`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_reference_for_mapping = REFERENCE_INDEXING.out.reference.map { meta, fasta, fai, dict, index ->
                                                                                          ^^^^
  ```

- Warning: `workflows/eager.nf:196:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(MAP.out.mqc.collect { it[1] }.ifEmpty([]))
                                                                    ^^
  ```

- Warning: `workflows/eager.nf:238:78`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FILTER_BAM.out.mqc.collect { it[1] }.ifEmpty([]))
                                                                               ^^
  ```

- Warning: `workflows/eager.nf:252:96`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta_for_deduplication = REFERENCE_INDEXING.out.reference.multiMap { meta, fasta, fai, dict, index ->
                                                                                                 ^^^^
  ```

- Warning: `workflows/eager.nf:252:102`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta_for_deduplication = REFERENCE_INDEXING.out.reference.multiMap { meta, fasta, fai, dict, index ->
                                                                                                       ^^^^^
  ```

- Warning: `workflows/eager.nf:275:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(MERGE_LIBRARIES.out.mqc.collect { it[1] }.ifEmpty([]))
                                                                                ^^
  ```

- Warning: `workflows/eager.nf:283:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              addNewMetaFromAttributes(it, "id", "reference", false)
                                       ^^
  ```

- Warning: `workflows/eager.nf:286:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, bam, bai ->
                                ^^^
  ```

- Warning: `workflows/eager.nf:290:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes(it, "reference", "reference", false)
                                           ^^
  ```

- Warning: `workflows/eager.nf:296:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch { ignore_meta, meta, bam, meta2, snp_capture_bed ->
                        ^^^^^^^^^^^
  ```

- Warning: `workflows/eager.nf:296:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch { ignore_meta, meta, bam, meta2, snp_capture_bed ->
                                     ^^^^
  ```

- Warning: `workflows/eager.nf:296:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch { ignore_meta, meta, bam, meta2, snp_capture_bed ->
                                           ^^^
  ```

- Warning: `workflows/eager.nf:296:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch { ignore_meta, meta, bam, meta2, snp_capture_bed ->
                                                ^^^^^
  ```

- Warning: `workflows/eager.nf:300:71`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_qualimap_input_with = ch_qualimap_input.withbed.multiMap { ignore_meta, meta, bam, meta2, snp_capture_bed ->
                                                                        ^^^^^^^^^^^
  ```

- Warning: `workflows/eager.nf:300:95`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_qualimap_input_with = ch_qualimap_input.withbed.multiMap { ignore_meta, meta, bam, meta2, snp_capture_bed ->
                                                                                                ^^^^^
  ```

- Warning: `workflows/eager.nf:306:67`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_qualimap_input_without = ch_qualimap_input.nobed.map { ignore_meta, meta, bam, meta2, snp_capture_bed ->
                                                                    ^^^^^^^^^^^
  ```

- Warning: `workflows/eager.nf:306:91`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_qualimap_input_without = ch_qualimap_input.nobed.map { ignore_meta, meta, bam, meta2, snp_capture_bed ->
                                                                                            ^^^^^
  ```

- Warning: `workflows/eager.nf:306:98`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_qualimap_input_without = ch_qualimap_input.nobed.map { ignore_meta, meta, bam, meta2, snp_capture_bed ->
                                                                                                   ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/eager.nf:311:9`: Variable was declared but not used

  ```nextflow
          ch_qualimap_output = QUALIMAP_BAMQC_WITHBED.out.results.mix(QUALIMAP_BAMQC_NOBED.out.results)
          ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/eager.nf:326:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def new_meta = meta.clone().findAll { it.key !in ['single_end', 'reference'] }
                                                        ^^
  ```

- Warning: `workflows/eager.nf:333:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def new_meta = meta.clone().findAll { it.key !in ['lane', 'colour_chemistry', 'single_end'] }
                                                    ^^
  ```

- Warning: `workflows/eager.nf:340:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta_join, meta_bam, bam, bai, meta_fastq, fastqs ->
                     ^^^^^^^^^
  ```

- Warning: `workflows/eager.nf:377:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              addNewMetaFromAttributes(it, "id", "reference", false)
                                       ^^
  ```

- Warning: `workflows/eager.nf:381:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes(it, "reference", "reference", false)
                                           ^^
  ```

- Warning: `workflows/eager.nf:387:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .multiMap { ignore_meta, meta, bam, bai, meta2, mito_header ->
                          ^^^^^^^^^^^
  ```

- Warning: `workflows/eager.nf:387:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .multiMap { ignore_meta, meta, bam, bai, meta2, mito_header ->
                                                  ^^^
  ```

- Warning: `workflows/eager.nf:392:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          MTNUCRATIO(mtnucratio_input.bam, mtnucratio_input.mito_header.map { it[1] })
                                                                              ^^
  ```

- Warning: `workflows/eager.nf:393:85`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(MTNUCRATIO.out.mtnucratio.collect { it[1] }.ifEmpty([]))
                                                                                      ^^
  ```

- Warning: `workflows/eager.nf:431:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(ENDORSPY.out.json.collect { it[1] }.ifEmpty([]))
                                                                          ^^
  ```

- Warning: `workflows/eager.nf:438:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          PRESEQ_CCURVE(ch_reads_for_deduplication.map { [it[0], it[1]] })
                                                          ^^
  ```

- Warning: `workflows/eager.nf:438:64`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          PRESEQ_CCURVE(ch_reads_for_deduplication.map { [it[0], it[1]] })
                                                                 ^^
  ```

- Warning: `workflows/eager.nf:439:85`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(PRESEQ_CCURVE.out.c_curve.collect { it[1] }.ifEmpty([]))
                                                                                      ^^
  ```

- Warning: `workflows/eager.nf:443:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          PRESEQ_LCEXTRAP(ch_reads_for_deduplication.map { [it[0], it[1]] })
                                                            ^^
  ```

- Warning: `workflows/eager.nf:443:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          PRESEQ_LCEXTRAP(ch_reads_for_deduplication.map { [it[0], it[1]] })
                                                                   ^^
  ```

- Warning: `workflows/eager.nf:444:89`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(PRESEQ_LCEXTRAP.out.lc_extrap.collect { it[1] }.ifEmpty([]))
                                                                                          ^^
  ```

- Warning: `workflows/eager.nf:455:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              addNewMetaFromAttributes(it, "id", "reference", false)
                                       ^^
  ```

- Warning: `workflows/eager.nf:460:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  addNewMetaFromAttributes(it, "reference", "reference", false)
                                           ^^
  ```

- Warning: `workflows/eager.nf:466:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { ignore_meta, meta, bam, bai, meta2, bedtools_feature ->
                     ^^^^^^^^^^^
  ```

- Warning: `workflows/eager.nf:466:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { ignore_meta, meta, bam, bai, meta2, bedtools_feature ->
                                                  ^^^^^
  ```

- Warning: `workflows/eager.nf:469:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch { meta, bedtools_feature, bam, bai ->
                        ^^^^
  ```

- Warning: `workflows/eager.nf:469:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch { meta, bedtools_feature, bam, bai ->
                                                ^^^
  ```

- Warning: `workflows/eager.nf:469:52`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch { meta, bedtools_feature, bam, bai ->
                                                     ^^^
  ```

- Warning: `workflows/eager.nf:495:100`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta_for_damagecalculation = REFERENCE_INDEXING.out.reference.multiMap { meta, fasta, fai, dict, index ->
                                                                                                     ^^^^
  ```

- Warning: `workflows/eager.nf:495:106`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta_for_damagecalculation = REFERENCE_INDEXING.out.reference.multiMap { meta, fasta, fai, dict, index ->
                                                                                                           ^^^^^
  ```

- Warning: `workflows/eager.nf:503:84`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(CALCULATE_DAMAGE.out.mqc.collect { it[1] }.ifEmpty([]))
                                                                                     ^^
  ```

- Warning: `workflows/eager.nf:515:85`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(RUN_SEXDETERRMINE.out.mqc.collect { it[1] }.ifEmpty([]))
                                                                                      ^^
  ```

- Warning: `workflows/eager.nf:527:90`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(ESTIMATE_CONTAMINATION.out.mqc.collect { it[1] }.ifEmpty([]))
                                                                                           ^^
  ```

- Warning: `workflows/eager.nf:536:90`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(MANIPULATE_DAMAGE.out.flagstat.collect { it[1] }.ifEmpty([]))
                                                                                           ^^
  ```

- Warning: `workflows/eager.nf:544:94`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(MERGE_LIBRARIES_GENOTYPING.out.mqc.collect { it[1] }.ifEmpty([]))
                                                                                               ^^
  ```

- Warning: `workflows/eager.nf:555:102`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_reference_for_genotyping = REFERENCE_INDEXING.out.reference.map { meta, fasta, fai, dict, mapindex ->
                                                                                                       ^^^^^^^^
  ```

- Warning: `workflows/eager.nf:566:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(GENOTYPE.out.mqc.collect { it[1] }.ifEmpty([]))
                                                                             ^^
  ```
