# Nextflow lint results

- Generated: 2026-07-21T00:30:03.727954822Z
- Nextflow version: 26.07.0-edge
- Summary: 23 warnings

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

- Warning: `subworkflows/local/utils_nfcore_methylseq_pipeline/main.nf:112:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, fastq_1, fastq_2, genome ->
                                         ^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_methylseq_pipeline/main.nf:235:9`: Variable was declared but not used

  ```nextflow
      def citation_text = ["Tools used in the workflow included:", "FastQC (Andrews 2010),", "Trim Galore! (Krueger)", "Bismark (Krueger 2011)", "bwa-meth (Pedersen 2014)", "Picard (Broad Institute 2019)", "Qualimap (Okonechnikov 2015)", "Preseq (Daley 2013)", "MultiQC (Ewels et al. 2016)", "."].join(' ').trim()
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

- Warning: `workflows/methylseq/main.nf:341:90`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(QUALIMAP_BAMQC.out.results.collect { it[1] }.ifEmpty([]))
                                                                                           ^^
  ```

- Warning: `workflows/methylseq/main.nf:344:87`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(PRESEQ_LCEXTRAP.out.log.collect { it[1] }.ifEmpty([]))
                                                                                        ^^
  ```

- Warning: `workflows/methylseq/main.nf:348:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(TRIMGALORE.out.log.collect { it[1] })
                                                                                   ^^
  ```

- Warning: `workflows/methylseq/main.nf:352:106`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_multiqc_files = ch_multiqc_files.mix(TARGETED_SEQUENCING.out.picard_metrics.collect { it[1] }.ifEmpty([]))
                                                                                                           ^^
  ```

- Warning: `workflows/methylseq/main.nf:356:78`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(FASTQC.out.zip.collect { it[1] }.ifEmpty([]))
                                                                               ^^
  ```
