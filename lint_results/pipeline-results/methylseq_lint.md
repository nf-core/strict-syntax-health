# Nextflow lint results

- Generated: 2026-07-15T00:25:05.504929273Z
- Nextflow version: 26.06.0-edge
- Summary: 2 errors, 31 warnings

## :x: Errors

- Error: `modules/nf-core/rastair/mbiasparser/main.nf:15:26`: `trim_OT` is not defined

  ```nextflow
      tuple val(meta), env(trim_OT), env(trim_OB),                    emit: mbias_processed_str
                           ^^^^^^^
  ```

- Error: `modules/nf-core/rastair/mbiasparser/main.nf:15:40`: `trim_OB` is not defined

  ```nextflow
      tuple val(meta), env(trim_OT), env(trim_OB),                    emit: mbias_processed_str
                                         ^^^^^^^
  ```

## :warning: Warnings

- Warning: `conf/modules/bismark_genomepreparation.config:9:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { it =~ /.*\.yml/ ? null : it },
                        ^^
  ```

- Warning: `conf/modules/bismark_genomepreparation.config:9:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { it =~ /.*\.yml/ ? null : it },
                                                 ^^
  ```

- Warning: `conf/modules/bwameth_index.config:7:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { it.equals('versions.yml') ? null : it.tokenize("/").last() },
                        ^^
  ```

- Warning: `conf/modules/bwameth_index.config:7:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { it.equals('versions.yml') ? null : it.tokenize("/").last() },
                                                           ^^
  ```

- Warning: `modules/nf-core/cat/fastq/main.nf:22:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def readList = reads instanceof List ? reads.collect { it.toString() } : [reads.toString()]
                                                             ^^
  ```

- Warning: `modules/nf-core/cat/fastq/main.nf:58:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def readList = reads instanceof List ? reads.collect { it.toString() } : [reads.toString()]
                                                             ^^
  ```

- Warning: `modules/nf-core/rastair/call/main.nf:25:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/rastair/mbias/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/trimgalore/main.nf:47:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          args_list.removeAll { it.toLowerCase().contains('_r2 ') }
                                ^^
  ```

- Warning: `subworkflows/local/targeted_sequencing/main.nf:29:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/targeted_sequencing/main.nf:30:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_picard_metrics = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/targeted_sequencing/main.nf:83:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_intervals = PICARD_BEDTOINTERVALLIST.out.intervallist.map { it[1] }
                                                                         ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_methylseq_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_methylseq_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_methylseq_pipeline/main.nf:109:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, fastq_1, fastq_2, genome ->
                                      ^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_methylseq_pipeline/main.nf:241:9`: Variable was declared but not used

  ```nextflow
      def citation_text = [
          ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_taps_conversion/main.nf:21:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_rastair_mbias = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_taps_conversion/main.nf:22:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_rastair_call  = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_taps_conversion/main.nf:23:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions      = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_taps_conversion/main.nf:47:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_rastair_mbiasparser.map{ meta, nOT_clip, nOB_clip -> [ meta, nOT_clip ] },
                                                      ^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_taps_conversion/main.nf:48:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_rastair_mbiasparser.map{ meta, nOT_clip, nOB_clip -> [ meta, nOB_clip ] },
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

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:101:98`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      return ch_versions.unique().map { version -> processVersionsFromYAML(version) }.unique().mix(Channel.of(workflowVersionToYAML()))
                                                                                                   ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:72:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/methylseq/main.nf:361:90`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(QUALIMAP_BAMQC.out.results.collect { it[1] }.ifEmpty([]))
                                                                                           ^^
  ```

- Warning: `workflows/methylseq/main.nf:364:87`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(PRESEQ_LCEXTRAP.out.log.collect { it[1] }.ifEmpty([]))
                                                                                        ^^
  ```

- Warning: `workflows/methylseq/main.nf:368:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(TRIMGALORE.out.log.collect { it[1] })
                                                                                   ^^
  ```

- Warning: `workflows/methylseq/main.nf:372:106`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_multiqc_files = ch_multiqc_files.mix(TARGETED_SEQUENCING.out.picard_metrics.collect { it[1] }.ifEmpty([]))
                                                                                                           ^^
  ```

- Warning: `workflows/methylseq/main.nf:376:78`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(FASTQC.out.zip.collect { it[1] }.ifEmpty([]))
                                                                               ^^
  ```
