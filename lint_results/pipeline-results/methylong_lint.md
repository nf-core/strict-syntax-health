# Nextflow lint results

- Generated: 2026-11-24T00:12:21.140732930Z
- Nextflow version: 26.11.0-edge
- Summary: 81 warnings

## :warning: Warnings

- Warning: `modules/local/bed2bedgraphs/ccsmeth_bedgraphs/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/bed2bedgraphs/modkit_bedgraphs/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/bed2bedgraphs/modkit_bedgraphs/main.nf:60:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/bed2bedgraphs/pbcpgtools_bedgraphs/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/bed2bedgraphs/pbcpgtools_bedgraphs/main.nf:39:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/ccsmeth/callfreqb/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/ccsmeth/callmods/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/dorado/aligner/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/dorado/aligner/main.nf:34:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/dorado/basecaller/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/dss/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/modkit/dmrpair/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/modkit/dmrpair/main.nf:28:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def a_params    = bed_hp1.collect { "-a $it" }.join(' ')
                                              ^^
  ```

- Warning: `modules/local/modkit/dmrpair/main.nf:29:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def b_params    = bed_hp2.collect { "-b $it" }.join(' ')
                                              ^^
  ```

- Warning: `modules/local/pb_cpg_tools/main.nf:41:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/rename_fastq/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/samtools/reset/main.nf:32:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/samtools/split_strands/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/samtools/split_strands/main.nf:37:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/whatshap/haplotag/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/whatshap/phase/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/clair3/main.nf:25:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/fastqc/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/fibertoolsrs/addnucleosomes/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/fibertoolsrs/extract/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/fibertoolsrs/predictm6a/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gawk/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gunzip/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gunzip/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/minimap2/align/main.nf:25:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/modkit/callmods/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/modkit/pileup/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/modkit/repair/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/multiqc/main.nf:24:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/pbjasmine/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/pbmm2/align/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/pbmm2/align/main.nf:41:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/pigz/compress/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/porechop/porechop/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/faidx/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/fastq/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/flagstat/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/import/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/index/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/sort/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/tabix/bgziptabix/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/tabix/tabix/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `subworkflows/local/ONT_main.nf:41:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it[1].toString().endsWith('.pod5') || file(it[1]).isDirectory() }
                    ^^
  ```

- Warning: `subworkflows/local/ONT_main.nf:41:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it[1].toString().endsWith('.pod5') || file(it[1]).isDirectory() }
                                                               ^^
  ```

- Warning: `subworkflows/local/ONT_main.nf:50:34`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .mix ( ch_input.filter { it[1].toString().endsWith('.bam') } )
                                   ^^
  ```

- Warning: `subworkflows/local/ONT_main.nf:57:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      map_stat = map_stat.mix(FASTQ_UNZIP.out.fastqc_log.collect { it[1] }.ifEmpty([]))
                                                                   ^^
  ```

- Warning: `subworkflows/local/Pacbio_main.nf:80:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      map_stat = map_stat.mix(FASTQ_UNZIP.out.fastqc_log.collect { it[1] }.ifEmpty([]))
                                                                   ^^
  ```

- Warning: `subworkflows/local/shared_bed2bedgraph/main.nf:25:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      modkit_input = in_bed.filter { it[0].method == 'ont' || (it[0].method == 'pacbio' && params.pileup_method == 'modkit') }
                                     ^^
  ```

- Warning: `subworkflows/local/shared_bed2bedgraph/main.nf:25:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      modkit_input = in_bed.filter { it[0].method == 'ont' || (it[0].method == 'pacbio' && params.pileup_method == 'modkit') }
                                                               ^^
  ```

- Warning: `subworkflows/local/shared_bed2bedgraph/main.nf:26:35`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      pbcpg_input = in_bed.filter { it[0].method == 'pacbio' && params.pileup_method == 'pbcpgtools' }
                                    ^^
  ```

- Warning: `subworkflows/local/shared_dss_population_scale/main.nf:43:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def metas = sampleList.collect { it[0] }
                                               ^^
  ```

- Warning: `subworkflows/local/shared_dss_population_scale/main.nf:44:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def beds  = sampleList.collect { it[1] }
                                               ^^
  ```

- Warning: `subworkflows/local/shared_dss_population_scale/main.nf:52:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def metas = sampleList.collect { it[0] }
                                               ^^
  ```

- Warning: `subworkflows/local/shared_dss_population_scale/main.nf:53:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def beds  = sampleList.collect { it[1] }
                                               ^^
  ```

- Warning: `subworkflows/local/shared_fastqc_unzip/main.nf:29:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      fastqc_log = fastqc_log.mix(FASTQC.out.zip.collect { it[1] }.ifEmpty([]))
                                                           ^^
  ```

- Warning: `subworkflows/local/shared_fastqc_unzip/main.nf:33:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it[1] =~ /fa\.gz$|fna\.gz$|fasta\.gz$/ }
                    ^^
  ```

- Warning: `subworkflows/local/shared_fastqc_unzip/main.nf:38:21`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { !(it[2] =~ /fa\.gz$|fna\.gz$|fasta\.gz$/) }
                      ^^
  ```

- Warning: `subworkflows/local/shared_gunzip_awk/main.nf:24:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it[1] =~ /\.vcf\.gz$/ }
                    ^^
  ```

- Warning: `subworkflows/local/shared_modkit_dmr_population_scale/main.nf:44:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def metas = sampleList.collect { it[0] }
                                               ^^
  ```

- Warning: `subworkflows/local/shared_modkit_dmr_population_scale/main.nf:45:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def beds  = sampleList.collect { it[1] }
                                               ^^
  ```

- Warning: `subworkflows/local/shared_modkit_dmr_population_scale/main.nf:46:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def tbis  = sampleList.collect { it[2] }
                                               ^^
  ```

- Warning: `subworkflows/local/shared_modkit_dmr_population_scale/main.nf:54:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def metas = sampleList.collect { it[0] }
                                               ^^
  ```

- Warning: `subworkflows/local/shared_modkit_dmr_population_scale/main.nf:55:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def beds  = sampleList.collect { it[1] }
                                               ^^
  ```

- Warning: `subworkflows/local/shared_modkit_dmr_population_scale/main.nf:56:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def tbis  = sampleList.collect { it[2] }
                                               ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_methylong_pipeline/main.nf:30:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_methylong_pipeline/main.nf:33:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_methylong_pipeline/main.nf:97:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_methylong_pipeline/main.nf:129:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      hook_url        //  string: hook URL for notifications
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_methylong_pipeline/main.nf:134:9`: Variable was declared but not used

  ```nextflow
      def multiqc_reports = multiqc_report.toList()
          ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/methylong.nf:58:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it[0].method == "pacbio" }
                    ^^
  ```

- Warning: `workflows/methylong.nf:62:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it[0].method == "ont" }
                    ^^
  ```

- Warning: `workflows/methylong.nf:71:75`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(PACBIO.out.map_stat.collect { it[1] }.ifEmpty([]))
                                                                            ^^
  ```

- Warning: `workflows/methylong.nf:76:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(ONT.out.map_stat.collect { it[1] }.ifEmpty([]))
                                                                         ^^
  ```

- Warning: `workflows/methylong.nf:126:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it != null &&!(it instanceof List && it.contains(null)) }
                    ^^
  ```

- Warning: `workflows/methylong.nf:126:34`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it != null &&!(it instanceof List && it.contains(null)) }
                                   ^^
  ```

- Warning: `workflows/methylong.nf:126:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it != null &&!(it instanceof List && it.contains(null)) }
                                                         ^^
  ```
