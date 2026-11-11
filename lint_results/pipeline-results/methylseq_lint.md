# Nextflow lint results

- Generated: 2026-11-11T00:15:41.757089102Z
- Nextflow version: 26.10.5
- Summary: 68 warnings

## :warning: Warnings

- Warning: `conf/modules/bismark_genomepreparation.config:12:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { it =~ /.*\.yml/ ? null : it },
                        ^^
  ```

- Warning: `conf/modules/bismark_genomepreparation.config:12:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

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

- Warning: `modules/local/filter_bedgraph_targets/main.nf:30:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bedtools/intersect/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bismark/align/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bismark/coverage2cytosine/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bismark/deduplicate/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bismark/genomepreparation/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bismark/methylationextractor/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bismark/report/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bismark/summary/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bwa/index/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bwa/mem/main.nf:25:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bwameth/align/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bwameth/index/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/cat/fastq/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
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

- Warning: `modules/nf-core/fastqc/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gunzip/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/methurator/gtestimator/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/methurator/plot/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/methyldackel/extract/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/methyldackel/mbias/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/multiqc/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/parabricks/fq2bam/main.nf:29:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/parabricks/fq2bammeth/main.nf:24:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/picard/addorreplacereadgroups/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/picard/bedtointervallist/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/picard/collecthsmetrics/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/picard/createsequencedictionary/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/picard/markduplicates/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/preseq/lcextrap/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/qualimap/bamqc/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/qualimap/bamqccram/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/rastair/call/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/rastair/call/main.nf:25:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/rastair/mbias/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/rastair/mbias/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/rastair/mbiasparser/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/rastair/methylkit/main.nf:16:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/faidx/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/flagstat/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/idxstats/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

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

- Warning: `modules/nf-core/samtools/stats/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/trimgalore/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/untar/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
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

- Warning: `subworkflows/local/utils_nfcore_methylseq_pipeline/main.nf:248:9`: Variable was declared but not used

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

- Warning: `workflows/methylseq/main.nf:323:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .combine(ch_fasta.map { meta, fasta -> fasta })
                                      ^^^^
  ```

- Warning: `workflows/methylseq/main.nf:324:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .combine(ch_fasta_index.map { meta, index -> index })
                                            ^^^^
  ```

- Warning: `workflows/methylseq/main.nf:377:90`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(QUALIMAP_BAMQC.out.results.collect { it[1] }.ifEmpty([]))
                                                                                           ^^
  ```

- Warning: `workflows/methylseq/main.nf:380:87`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(PRESEQ_LCEXTRAP.out.log.collect { it[1] }.ifEmpty([]))
                                                                                        ^^
  ```

- Warning: `workflows/methylseq/main.nf:384:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(TRIMGALORE.out.log.collect { it[1] })
                                                                                   ^^
  ```

- Warning: `workflows/methylseq/main.nf:388:106`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_multiqc_files = ch_multiqc_files.mix(TARGETED_SEQUENCING.out.picard_metrics.collect { it[1] }.ifEmpty([]))
                                                                                                           ^^
  ```

- Warning: `workflows/methylseq/main.nf:392:78`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(FASTQC.out.zip.collect { it[1] }.ifEmpty([]))
                                                                               ^^
  ```
