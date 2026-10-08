# Nextflow lint results

- Generated: 2026-10-08T00:23:45.737713137Z
- Nextflow version: 26.09.2-edge
- Summary: 45 warnings

## :warning: Warnings

- Warning: `modules/local/custom/filterbed/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/custom/joinbed/main.nf:20:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/custom/stripheader/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/episegmix/dmdecode/main.nf:33:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/episegmix/dmreport/main.nf:33:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/episegmix/dnadecode/main.nf:32:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${sample_id}"
          ^^^^^^
  ```

- Warning: `modules/local/episegmix/dnareport/main.nf:33:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${sample_id}"
          ^^^^^^
  ```

- Warning: `modules/local/episegmix/ldmdecode/main.nf:32:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${sample_id}"
          ^^^^^^
  ```

- Warning: `modules/local/episegmix/ldmreport/main.nf:33:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/episegmix/traincounts/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/bam_reheader_index_samtools/main.nf:10:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/bed_counts/main.nf:19:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta1, chrombin, meta2, tab ->
                 ^^^^^
  ```

- Warning: `subworkflows/local/bed_counts/main.nf:22:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_dummy_chrom_sizes = Channel.value([ [id: 'dummy'], [] ])
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/episegmix_fitting/main.nf:12:12`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .map { sample_id, log -> log }
             ^^^^^^^^^
  ```

- Warning: `subworkflows/local/episegmix_fitting/main.nf:15:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_input = Channel.fromPath(params.input)
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/merge/main.nf:15:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          sample_id, meta1, histone, meta3 , binned ->
                     ^^^^^
  ```

- Warning: `subworkflows/local/merge/main.nf:15:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          sample_id, meta1, histone, meta3 , binned ->
                                     ^^^^^
  ```

- Warning: `subworkflows/local/merge/main.nf:15:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          sample_id, meta1, histone, meta3 , binned ->
                                             ^^^^^^
  ```

- Warning: `subworkflows/local/merge/main.nf:28:9`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          sample_id, meta1, histone, meta3, binned, noheaderhistone ->
          ^^^^^^^^^
  ```

- Warning: `subworkflows/local/merge/main.nf:28:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          sample_id, meta1, histone, meta3, binned, noheaderhistone ->
                     ^^^^^
  ```

- Warning: `subworkflows/local/merge/main.nf:28:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          sample_id, meta1, histone, meta3, binned, noheaderhistone ->
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/merge/main.nf:36:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_chrom_dummy = Channel.value([ [id: "DUMMY"], [] ])
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:8:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:19:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_raw_chromsizes = Channel.fromPath(params.chromsizes)
                              ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_epigenomesegmentation_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:37:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def ch_versions = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:50:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_in_bam_reheader = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:60:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_histonecounts = Channel.fromPath(params.histonecounts).first()
                             ^^^^^^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:61:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_methcounts    = Channel.fromPath(params.methcounts).first()
                             ^^^^^^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:63:26`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, bamfile -> [meta.id, meta] }
                           ^^^^^^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:70:26`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, bedfile -> [meta.id, meta] }
                           ^^^^^^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:78:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_histonecounts = Channel.fromPath(params.histonecounts).first()
                             ^^^^^^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:80:26`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, bamfile -> [meta.id, meta] }
                           ^^^^^^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:85:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_meth_tab =  Channel.empty()
                         ^^^^^^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:92:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_methcounts = Channel.fromPath(params.methcounts).first()
                          ^^^^^^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:94:26`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, bedfile -> [meta.id, meta] }
                           ^^^^^^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:125:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_states = Channel.of("${params.states}").splitCsv().flatten()
                  ^^^^^^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:145:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_dist = Channel.of("${params.distributions}").splitCsv().flatten()
                    ^^^^^^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:180:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { sample_id, meta1, histone, meta2, meth, state, dist ->
                     ^^^^^^^^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:180:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { sample_id, meta1, histone, meta2, meth, state, dist ->
                                                ^^^^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:180:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { sample_id, meta1, histone, meta2, meth, state, dist ->
                                                       ^^^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:197:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_in_episegmix_config = Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:238:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                              def histone_files = histone.flatten().findAll { it != null }
                                                                              ^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:239:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                              def meth_files = meth.flatten().findAll { it != null }
                                                                        ^^
  ```

- Warning: `workflows/epigenomesegmentation.nf:321:9`: Variable was declared but not used

  ```nextflow
      def ch_collated_versions = softwareVersionsToYAML(ch_versions.mix(topic_versions.versions_file))
          ^^^^^^^^^^^^^^^^^^^^
  ```
