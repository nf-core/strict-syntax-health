# Nextflow lint results

- Generated: 2026-05-05T00:32:22.757324040Z
- Nextflow version: 26.04.0
- Summary: 51 errors, 44 warnings

## :x: Errors

- Error: `modules/local/write_sample_list/main.nf:16:48`: `PWD` is not defined

  ```nextflow
          line="${meta.id},${meta.single_end},[${PWD}/${params.outdir}/bigwig/${bw_or_bam[0]} ${PWD}/${params.outdir}/bigwig/${bw_or_bam[1]}],${meta.id}"
                                                 ^^^
  ```

- Error: `modules/local/write_sample_list/main.nf:16:95`: `PWD` is not defined

  ```nextflow
          line="${meta.id},${meta.single_end},[${PWD}/${params.outdir}/bigwig/${bw_or_bam[0]} ${PWD}/${params.outdir}/bigwig/${bw_or_bam[1]}],${meta.id}"
                                                                                                ^^^
  ```

- Error: `modules/local/write_sample_list/main.nf:21:47`: `PWD` is not defined

  ```nextflow
          line="${meta.id},${meta.single_end},${PWD}/${params.outdir}/samtools_sort/${bw_or_bam[0]},${meta.id}"
                                                ^^^
  ```

- Error: `subworkflows/local/cager/main.nf:93:5`: `id` was assigned but not declared

  ```nextflow
      id = row.id
      ^^
  ```

- Error: `subworkflows/local/cager/main.nf:94:5`: `single_end` was assigned but not declared

  ```nextflow
      single_end = row.single_end
      ^^^^^^^^^^
  ```

- Error: `subworkflows/local/cager/main.nf:95:5`: `str1_bw` was assigned but not declared

  ```nextflow
      str1_bw = row.path.split(" ")[0].minus('[')
      ^^^^^^^
  ```

- Error: `subworkflows/local/cager/main.nf:96:5`: `new_name` was assigned but not declared

  ```nextflow
      new_name = row.new_name
      ^^^^^^^^
  ```

- Error: `subworkflows/local/cager/main.nf:97:9`: `str1_bw` is not defined

  ```nextflow
      if (str1_bw.split("\\.")[-1].minus(']') != "bam") {
          ^^^^^^^
  ```

- Error: `subworkflows/local/cager/main.nf:98:9`: `str2_bw` was assigned but not declared

  ```nextflow
          str2_bw = row.path.split(" ")[1].minus(']')
          ^^^^^^^
  ```

- Error: `subworkflows/local/cager/main.nf:99:17`: `id` is not defined

  ```nextflow
          return [id, single_end, str1_bw, str2_bw, new_name]
                  ^^
  ```

- Error: `subworkflows/local/cager/main.nf:99:21`: `single_end` is not defined

  ```nextflow
          return [id, single_end, str1_bw, str2_bw, new_name]
                      ^^^^^^^^^^
  ```

- Error: `subworkflows/local/cager/main.nf:99:33`: `str1_bw` is not defined

  ```nextflow
          return [id, single_end, str1_bw, str2_bw, new_name]
                                  ^^^^^^^
  ```

- Error: `subworkflows/local/cager/main.nf:99:42`: `str2_bw` is not defined

  ```nextflow
          return [id, single_end, str1_bw, str2_bw, new_name]
                                           ^^^^^^^
  ```

- Error: `subworkflows/local/cager/main.nf:99:51`: `new_name` is not defined

  ```nextflow
          return [id, single_end, str1_bw, str2_bw, new_name]
                                                    ^^^^^^^^
  ```

- Error: `subworkflows/local/cager/main.nf:101:13`: `id` is not defined

  ```nextflow
      return [id, single_end, str1_bw, new_name]
              ^^
  ```

- Error: `subworkflows/local/cager/main.nf:101:17`: `single_end` is not defined

  ```nextflow
      return [id, single_end, str1_bw, new_name]
                  ^^^^^^^^^^
  ```

- Error: `subworkflows/local/cager/main.nf:101:29`: `str1_bw` is not defined

  ```nextflow
      return [id, single_end, str1_bw, new_name]
                              ^^^^^^^
  ```

- Error: `subworkflows/local/cager/main.nf:101:38`: `new_name` is not defined

  ```nextflow
      return [id, single_end, str1_bw, new_name]
                                       ^^^^^^^^
  ```

- Error: `subworkflows/local/deduplication/main.nf:22:9`: Incorrect number of call arguments, expected 3 but received 1

  ```nextflow
          SORT_FOR_FIXMATE (
          ^
  ```

- Error: `subworkflows/local/deduplication/main.nf:30:9`: Incorrect number of call arguments, expected 3 but received 1

  ```nextflow
          SORT_AFTER_FIXMATE(ch_bam_to_sort)
          ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/input_from_folder/main.nf:30:17`: Variables in a closure should be declared with `def`

  ```nextflow
                  num_fields_of_interest = "$params.sample_name_fields".toInteger()
                  ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/input_from_folder/main.nf:31:17`: Variables in a closure should be declared with `def`

  ```nextflow
                  split_field_num = old_meta.split('_').size()
                  ^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/input_from_folder/main.nf:33:21`: Variables in a closure should be declared with `def`

  ```nextflow
                      sample_name = old_meta
                      ^^^^^^^^^^^
  ```

- Error: `subworkflows/local/input_from_folder/main.nf:34:21`: Variables in a closure should be declared with `def`

  ```nextflow
                      lane_n_fastq = tuple(fastq.name, fastq)
                      ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/input_from_folder/main.nf:36:21`: Variables in a closure should be declared with `def`

  ```nextflow
                      num_fields_to_cut = split_field_num - num_fields_of_interest
                      ^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/input_from_folder/main.nf:46:19`: `lane_n_fastq` is already declared

  ```nextflow
              meta, lane_n_fastq ->
                    ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/input_from_folder/main.nf:48:17`: Variables in a closure should be declared with `def`

  ```nextflow
                  fastq = lane_n_fastq*.getAt(1).flatten()
                  ^^^^^
  ```

- Error: `subworkflows/local/mapped_inputs/main.nf:19:5`: `files_in` was assigned but not declared

  ```nextflow
      files_in = row.path
      ^^^^^^^^
  ```

- Error: `subworkflows/local/mapped_inputs/main.nf:20:5`: `files` was assigned but not declared

  ```nextflow
      files = files_in.split(' ')
      ^^^^^
  ```

- Error: `subworkflows/local/mapped_inputs/main.nf:20:13`: `files_in` is not defined

  ```nextflow
      files = files_in.split(' ')
              ^^^^^^^^
  ```

- Error: `subworkflows/local/mapped_inputs/main.nf:21:9`: `files` is not defined

  ```nextflow
      if (files.size() == 2){
          ^^^^^
  ```

- Error: `subworkflows/local/mapped_inputs/main.nf:22:9`: `bigwig_1` was assigned but not declared

  ```nextflow
          bigwig_1 = file(files[0].minus('['))
          ^^^^^^^^
  ```

- Error: `subworkflows/local/mapped_inputs/main.nf:22:25`: `files` is not defined

  ```nextflow
          bigwig_1 = file(files[0].minus('['))
                          ^^^^^
  ```

- Error: `subworkflows/local/mapped_inputs/main.nf:23:9`: `bigwig_2` was assigned but not declared

  ```nextflow
          bigwig_2 = file(files[1].minus(']'))
          ^^^^^^^^
  ```

- Error: `subworkflows/local/mapped_inputs/main.nf:23:25`: `files` is not defined

  ```nextflow
          bigwig_2 = file(files[1].minus(']'))
                          ^^^^^
  ```

- Error: `subworkflows/local/mapped_inputs/main.nf:24:17`: `bigwig_1` is not defined

  ```nextflow
          return [bigwig_1, bigwig_2]
                  ^^^^^^^^
  ```

- Error: `subworkflows/local/mapped_inputs/main.nf:24:27`: `bigwig_2` is not defined

  ```nextflow
          return [bigwig_1, bigwig_2]
                            ^^^^^^^^
  ```

- Error: `subworkflows/local/mapped_inputs/main.nf:25:16`: `files` is not defined

  ```nextflow
      } else if (files.size() == 1){
                 ^^^^^
  ```

- Error: `subworkflows/local/mapped_inputs/main.nf:26:9`: `bam` was assigned but not declared

  ```nextflow
          bam = file(files[0].minus('[').minus(']'))
          ^^^
  ```

- Error: `subworkflows/local/mapped_inputs/main.nf:26:20`: `files` is not defined

  ```nextflow
          bam = file(files[0].minus('[').minus(']'))
                     ^^^^^
  ```

- Error: `subworkflows/local/mapped_inputs/main.nf:27:17`: `bam` is not defined

  ```nextflow
          return [bam]
                  ^^^
  ```

- Error: `subworkflows/local/star/main.nf:55:51`: `wigs` is already declared

  ```nextflow
              wigs_for_conversion = wigs.map{ meta, wigs ->
                                                    ^^^^
  ```

- Error: `subworkflows/local/star/main.nf:57:17`: Variables in a closure should be declared with `def`

  ```nextflow
                  wigs_to_use = [wigs[0], wigs[1]]
                  ^^^^^^^^^^^
  ```

- Error: `subworkflows/local/star/main.nf:61:51`: `wigs` is already declared

  ```nextflow
              wigs_for_conversion = wigs.map{ meta, wigs ->
                                                    ^^^^
  ```

- Error: `workflows/cageseq.nf:18:1`: Invalid include source: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/cageseq/subworkflows/local/parameter_checks/main.nf'

  ```nextflow
  include { PARAMETER_CHECKS } from '../subworkflows/local/parameter_checks/main.nf'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/cageseq.nf:66:9`: `PARAMETER_CHECKS` is not defined

  ```nextflow
          PARAMETER_CHECKS(ch_fasta, ch_index)
          ^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/cageseq.nf:68:20`: `PARAMETER_CHECKS` is not defined

  ```nextflow
          ch_fasta = PARAMETER_CHECKS.out.ch_fasta
                     ^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/cageseq.nf:69:20`: `PARAMETER_CHECKS` is not defined

  ```nextflow
          ch_index = PARAMETER_CHECKS.out.ch_index
                     ^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/cageseq.nf:70:20`: `PARAMETER_CHECKS` is not defined

  ```nextflow
          ch_fastq = PARAMETER_CHECKS.out.ch_fastq
                     ^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/cageseq.nf:122:17`: Variables in a closure should be declared with `def`

  ```nextflow
                  file1 = paths[0]
                  ^^^^^
  ```

- Error: `workflows/cageseq.nf:123:17`: Variables in a closure should be declared with `def`

  ```nextflow
                  file2 = paths[1]
                  ^^^^^
  ```

## :warning: Warnings

- Warning: `modules/nf-core/ucsc/wigtobigwig/main.nf:47:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `subworkflows/local/bowtie2/main.nf:18:52`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          sample_meta = ch_reads_to_align.map{ meta, fastq ->
                                                     ^^^^^
  ```

- Warning: `subworkflows/local/bowtie2/main.nf:26:74`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_index = sample_meta.combine(BOWTIE2_BUILD.out.index.map { genome_name, index -> index } )
                                                                           ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bowtie2/main.nf:28:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_index = sample_meta.combine(ch_index.map { genome_name, index -> index })
                                                            ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bowtie2/main.nf:32:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_fasta = sample_meta.combine(ch_fasta.map { genome_name, fasta -> fasta } )
                                                            ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bowtie2/main.nf:44:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(BOWTIE2_ALIGN.out.log.collect{it[1]})
                                                                                ^^
  ```

- Warning: `subworkflows/local/bowtie2/main.nf:53:9`: Variable was declared but not used

  ```nextflow
          ch_aligned = SAMTOOLS_VIEW.out.bam
          ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/cager/main.nf:26:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_data_type = Channel.of("bam")
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/cager/main.nf:28:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_data_type = Channel.of(params.datatype)
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/cager/main.nf:33:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { create_mapping_channel(it) }
                                            ^^
  ```

- Warning: `subworkflows/local/cager/main.nf:74:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_template = Channel.fromPath(params.markdown_path)
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/cager/main.nf:76:9`: Variable was declared but not used

  ```nextflow
          ch_html = CAGER_REPORT(
          ^^^^^^^
  ```

- Warning: `subworkflows/local/deduplication/main.nf:47:9`: Variable was declared but not used

  ```nextflow
          ch_bam_bai = SAMTOOLS_MARKDUP.out.bam.join(INDEX_DEDUP.out.bai)
          ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/input_from_folder/main.nf:23:5`: Variable was declared but not used

  ```nextflow
      ch_fastq = channel
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/mapped_inputs/main.nf:10:5`: Variable was declared but not used

  ```nextflow
      input_files = sample_file
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/mapped_inputs/main.nf:12:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { create_sample_channel(it) }
                                       ^^
  ```

- Warning: `subworkflows/local/prepare_cager_metadata/main.nf:18:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              seqs_fasta = Channel.fromPath("${params.sourcedir}/*", checkIfExists: true).collect()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_cager_metadata/main.nf:20:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  Channel.value([[id: 'bsgenome'], forge_seed]),
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_cager_metadata/main.nf:37:64`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_bsgenome_file = FORGEBSGENOME.out.tarball.map { meta, tarball -> tarball }
                                                                 ^^^^
  ```

- Warning: `subworkflows/local/prepare_cager_metadata/main.nf:41:9`: Variable was declared but not used

  ```nextflow
          ch_txdb = GTF2TXDB(ch_gtf)
          ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_cager_metadata/main.nf:42:9`: Variable was declared but not used

  ```nextflow
          ch_txdb_file = GTF2TXDB.out.txdb
          ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_mapping_metadata/main.nf:17:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              chrom_size_fa = ch_fasta.map{ meta, fasta ->
                                            ^^^^
  ```

- Warning: `subworkflows/local/prepare_mapping_metadata/main.nf:30:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_chrom_sizes = Channel.of([
                               ^^^^^^^
  ```

- Warning: `subworkflows/local/preprocessing/main.nf:40:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTQC.out.zip.collect{it[1]}.ifEmpty([]))
                                                                         ^^
  ```

- Warning: `subworkflows/local/preprocessing/main.nf:41:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(TRIMGALORE.out.log.collect{it[1]}.ifEmpty([]))
                                                                             ^^
  ```

- Warning: `subworkflows/local/preprocessing/main.nf:42:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(TRIMGALORE.out.zip.collect{it[1]}.ifEmpty([]))
                                                                             ^^
  ```

- Warning: `subworkflows/local/preprocessing/main.nf:43:9`: Variable was declared but not used

  ```nextflow
          ch_reads_to_align = !params.nogtrim ? CUTADAPT.out.reads : TRIMGALORE.out.reads
          ^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/samtools/main.nf:16:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_index_format = Channel.value("bai")
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/samtools/main.nf:20:9`: Variable was declared but not used

  ```nextflow
          ch_bam_bai = SAMTOOLS_SORT.out.bam.join(SAMTOOLS_INDEX.out.bai)
          ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/star/main.nf:21:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_genome_name = Channel.of(params.genome_name)
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/star/main.nf:23:52`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          sample_meta = ch_reads_to_align.map{ meta, fastq ->
                                                     ^^^^^
  ```

- Warning: `subworkflows/local/star/main.nf:32:80`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_index = sample_meta.combine(STAR_GENOMEGENERATE.out.index.map { it[1] })
                                                                                 ^^
  ```

- Warning: `subworkflows/local/star/main.nf:44:9`: Variable was declared but not used

  ```nextflow
          ch_aligned = STAR_ALIGN.out.bam_sorted_aligned
          ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/star/main.nf:46:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(STAR_ALIGN.out.log_final.collect{it[1]})
                                                                                   ^^
  ```

- Warning: `subworkflows/local/star/main.nf:48:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_chrom_sizes_for_wig = ch_chrom_sizes.map{meta, sizes ->
                                                      ^^^^
  ```

- Warning: `subworkflows/local/star/main.nf:73:9`: Variable was declared but not used

  ```nextflow
          bigwig_ch_for_cager = UCSC_WIGTOBIGWIG.out.bw
          ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_cageseq_pipeline/main.nf:33:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_cageseq_pipeline/main.nf:36:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```

- Warning: `workflows/cageseq.nf:40:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_samplesheet // channel: samplesheet read in from --input
      ^^^^^^^^^^^^^^
  ```

- Warning: `workflows/cageseq.nf:112:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it[3], it[4]]}
                    ^^
  ```

- Warning: `workflows/cageseq.nf:112:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{[it[3], it[4]]}
                           ^^
  ```

- Warning: `workflows/cageseq.nf:117:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              mapped_files_ch = ch_for_cager.map{ meta, paths ->
                                                  ^^^^
  ```

- Warning: `workflows/cageseq.nf:121:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              mapped_files_ch = ch_for_cager.map{ meta, paths ->
                                                  ^^^^
  ```
