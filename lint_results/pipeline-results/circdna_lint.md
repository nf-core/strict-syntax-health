# Nextflow lint results

- Generated: 2026-06-30T00:39:32.138512364Z
- Nextflow version: 26.05.0-edge
- Summary: 4 errors, 62 warnings

## :x: Errors

- Error: `subworkflows/local/input_check/main.nf:5:1`: Invalid include source: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/circdna/subworkflows/modules/local/samplesheet_check.nf'

  ```nextflow
  include { SAMPLESHEET_CHECK } from '../../modules/local/samplesheet_check'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/input_check/main.nf:13:9`: `SAMPLESHEET_CHECK` is not defined

  ```nextflow
          SAMPLESHEET_CHECK ( samplesheet )
          ^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/input_check/main.nf:19:9`: `SAMPLESHEET_CHECK` is not defined

  ```nextflow
          SAMPLESHEET_CHECK ( samplesheet )
          ^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/input_check/main.nf:31:16`: `SAMPLESHEET_CHECK` is not defined

  ```nextflow
      versions = SAMPLESHEET_CHECK.out.versions // channel: [ versions.yml ]
                 ^^^^^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `main.nf:61:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = CIRCDNA.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/ampliconsuite/main.nf:34:9`: Variable was declared but not used

  ```nextflow
      def cngain = params.aa_cngain
          ^^^^^^
  ```

- Warning: `modules/local/ampliconsuite/main.nf:64:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/ampliconsuite/main.nf:66:9`: Variable was declared but not used

  ```nextflow
      def cngain = params.aa_cngain
          ^^^^^^
  ```

- Warning: `modules/local/ampliconsuite/main.nf:67:9`: Variable was declared but not used

  ```nextflow
      def ref = params.reference_build
          ^^^
  ```

- Warning: `modules/local/bwa/mem/main.nf:45:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/bwa/mem/main.nf:46:9`: Variable was declared but not used

  ```nextflow
      def args2 = task.ext.args2 ?: ''
          ^^^^^
  ```

- Warning: `modules/local/bwa/mem/main.nf:48:9`: Variable was declared but not used

  ```nextflow
      def samtools_command = sort_bam ? 'sort' : 'view'
          ^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/circlefinder/main.nf:16:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/circlemap/readextractor/main.nf:18:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/getcircularreads/main.nf:15:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/samtools/flagstat/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/samtools/idxstats/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/input_check/main.nf:16:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { create_fastq_channels(it) }
                                           ^^
  ```

- Warning: `subworkflows/local/input_check/main.nf:22:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { create_bam_channels(it) }
                                         ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_circdna_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_circdna_pipeline/main.nf:111:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel
          ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_circdna_pipeline/main.nf:135:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel
          ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_circdna_pipeline/main.nf:146:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { id, metas, bams ->
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

- Warning: `workflows/circdna.nf:88:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/circdna.nf:89:5`: Variable was declared but not used

  ```nextflow
      ch_versions_topic = Channel.topic('versions')
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/circdna.nf:89:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions_topic = Channel.topic('versions')
                          ^^^^^^^
  ```

- Warning: `workflows/circdna.nf:93:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      multiqc_report = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `workflows/circdna.nf:97:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_fasta = Channel.fromPath(params.fasta)
                     ^^^^^^^
  ```

- Warning: `workflows/circdna.nf:120:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_bwa_index = Channel.fromPath(params.bwa_index, type: 'dir').collect()
                         ^^^^^^^
  ```

- Warning: `workflows/circdna.nf:124:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_bwa_index = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `workflows/circdna.nf:133:9`: Variable was declared but not used

  ```nextflow
          mosek_license_dir = file(params.mosek_license_dir)
          ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/circdna.nf:148:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_samtools_stats           = Channel.empty()
                                    ^^^^^^^
  ```

- Warning: `workflows/circdna.nf:149:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_samtools_flagstat        = Channel.empty()
                                    ^^^^^^^
  ```

- Warning: `workflows/circdna.nf:150:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_samtools_idxstats        = Channel.empty()
                                    ^^^^^^^
  ```

- Warning: `workflows/circdna.nf:151:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_markduplicates_stats     = Channel.empty()
                                    ^^^^^^^
  ```

- Warning: `workflows/circdna.nf:152:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_markduplicates_flagstat  = Channel.empty()
                                    ^^^^^^^
  ```

- Warning: `workflows/circdna.nf:153:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_markduplicates_idxstats  = Channel.empty()
                                    ^^^^^^^
  ```

- Warning: `workflows/circdna.nf:154:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_markduplicates_multiqc   = Channel.empty()
                                    ^^^^^^^
  ```

- Warning: `workflows/circdna.nf:193:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_fastqc_multiqc = Channel.empty()
                              ^^^^^^^
  ```

- Warning: `workflows/circdna.nf:213:43`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_trimgalore_multiqc       = Channel.empty()
                                            ^^^^^^^
  ```

- Warning: `workflows/circdna.nf:214:43`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_trimgalore_multiqc_log   = Channel.empty()
                                            ^^^^^^^
  ```

- Warning: `workflows/circdna.nf:226:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_bwa_index = BWA_INDEX.out.index.map{ meta, index -> ["bwa_index", index] }.collect()
                                                      ^^^^
  ```

- Warning: `workflows/circdna.nf:239:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  Channel.value(true)
                  ^^^^^^^
  ```

- Warning: `workflows/circdna.nf:277:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_fastqc_multiqc           = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `workflows/circdna.nf:278:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_trimgalore_multiqc       = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `workflows/circdna.nf:279:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_trimgalore_multiqc_log   = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `workflows/circdna.nf:293:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_fasta = ch_fasta_meta.map{ meta, index -> [index] }.collect()
                                        ^^^^
  ```

- Warning: `workflows/circdna.nf:364:51`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ch_markduplicates_stats         = Channel.empty()
                                                    ^^^^^^^
  ```

- Warning: `workflows/circdna.nf:365:51`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ch_markduplicates_flagstat      = Channel.empty()
                                                    ^^^^^^^
  ```

- Warning: `workflows/circdna.nf:366:51`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ch_markduplicates_idxstats      = Channel.empty()
                                                    ^^^^^^^
  ```

- Warning: `workflows/circdna.nf:367:51`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ch_markduplicates_multiqc       = Channel.empty()
                                                    ^^^^^^^
  ```

- Warning: `workflows/circdna.nf:467:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, bam, bai -> [meta, bam] }
                                ^^^
  ```

- Warning: `workflows/circdna.nf:550:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def ch_multiqc_files = ch_fastqc_multiqc.collect{it[1]}.ifEmpty([])
                                                           ^^
  ```

- Warning: `workflows/circdna.nf:551:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .mix(ch_trimgalore_multiqc.collect{it[1]}.ifEmpty([]))
                                                 ^^
  ```

- Warning: `workflows/circdna.nf:552:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .mix(ch_trimgalore_multiqc_log.collect{it[1]}.ifEmpty([]))
                                                     ^^
  ```

- Warning: `workflows/circdna.nf:553:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .mix(ch_samtools_stats.collect{it[1]}.ifEmpty([]))
                                             ^^
  ```

- Warning: `workflows/circdna.nf:554:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .mix(ch_samtools_flagstat.collect{it[1]}.ifEmpty([]))
                                                ^^
  ```

- Warning: `workflows/circdna.nf:555:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .mix(ch_samtools_idxstats.collect{it[1]}.ifEmpty([]))
                                                ^^
  ```

- Warning: `workflows/circdna.nf:556:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .mix(ch_markduplicates_stats.collect{it[1]}.ifEmpty([]))
                                                   ^^
  ```

- Warning: `workflows/circdna.nf:557:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .mix(ch_markduplicates_flagstat.collect{it[1]}.ifEmpty([]))
                                                      ^^
  ```

- Warning: `workflows/circdna.nf:558:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .mix(ch_markduplicates_idxstats.collect{it[1]}.ifEmpty([]))
                                                      ^^
  ```

- Warning: `workflows/circdna.nf:559:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .mix(ch_markduplicates_multiqc.collect{it[1]}.ifEmpty([]))
                                                     ^^
  ```

- Warning: `workflows/circdna.nf:582:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = multiqc_report
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```
