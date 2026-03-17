# Nextflow lint results

- Generated: 2026-03-17T00:23:59.326185297Z
- Nextflow version: 26.02.0-edge
- Summary: 177 warnings

## :warning: Warnings

- Warning: `conf/modules.config:496:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          return args_list.findAll { it }.join(' ').trim()
                                     ^^
  ```

- Warning: `main.nf:59:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.empty() // FIXED: Added missing multiqc_report parameter
          ^^^^^^^
  ```

- Warning: `modules/local/fix_header_sv/cutesv/main.nf:19:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/fix_header_sv/jasmine/main.nf:19:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/rtg/mendelian/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/rtg/mendelian_violations/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/sniffles/trio/main.nf:18:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def snf_input = snf_files.collect{ it.toString() }.join(' ')
                                         ^^
  ```

- Warning: `modules/local/straglr/main.nf:39:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/svanna/main.nf:28:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          hpo_args = hpo_terms.split(';').collect { "--phenotype-term ${it}" }.join(' ')
                                                                        ^^
  ```

- Warning: `modules/nf-core/bcftools/concat/main.nf:32:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input = vcfs.sort{it.toString()}.join(" ")
                            ^^
  ```

- Warning: `modules/nf-core/bcftools/merge/main.nf:28:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input = (vcfs.collect().size() > 1) ? vcfs.sort{ it.name } : vcfs
                                                           ^^
  ```

- Warning: `modules/nf-core/bcftools/norm/main.nf:56:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          if (['--write-index=tbi', '-W=tbi'].any { args.contains(it) }  && extension == 'vcf.gz') {
                                                                  ^^
  ```

- Warning: `modules/nf-core/bcftools/norm/main.nf:58:126`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          } else if (['--write-index=tbi', '-W=tbi', '--write-index=csi', '-W=csi', '--write-index', '-W'].any { args.contains(it) }) {
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

- Warning: `modules/nf-core/clair3/main.nf:72:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/deepvariant/vcfstatsreport/main.nf:25:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/glnexus/main.nf:27:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input = gvcfs.collect { it.toString() }
                                  ^^
  ```

- Warning: `modules/nf-core/gunzip/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/jasminesv/main.nf:37:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def unzip_inputs = vcfs.collect { it.name.endsWith(".vcf.gz") ? "    bgzip -d --threads ${task.cpus} ${args4} ${it}" : "" }.join("\n")
                                        ^^
  ```

- Warning: `modules/nf-core/jasminesv/main.nf:37:117`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def unzip_inputs = vcfs.collect { it.name.endsWith(".vcf.gz") ? "    bgzip -d --threads ${task.cpus} ${args4} ${it}" : "" }.join("\n")
                                                                                                                      ^^
  ```

- Warning: `modules/nf-core/minimap2/align/main.nf:67:9`: Variable was declared but not used

  ```nextflow
      def target = reference ?: (bam_input ? error("BAM input requires reference") : reads)
          ^^^^^^
  ```

- Warning: `modules/nf-core/modkit/pileup/main.nf:58:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/align/main.nf:17:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/align/main.nf:42:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta_sample, reads, meta_ref, index ->
                                         ^^^^^^^^
  ```

- Warning: `subworkflows/local/align/main.nf:54:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_align_input.map { meta_sample, reads, meta_index, index ->
                                                       ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/align/main.nf:54:66`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_align_input.map { meta_sample, reads, meta_index, index ->
                                                                   ^^^^^
  ```

- Warning: `subworkflows/local/align/main.nf:57:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_align_input.map { meta_sample, reads, meta_index, index ->
                                   ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/align/main.nf:57:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_align_input.map { meta_sample, reads, meta_index, index ->
                                                ^^^^^
  ```

- Warning: `subworkflows/local/annotate_sniffles/main.nf:17:44`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_candidate_genes = candidate_genes ? Channel.fromPath(candidate_genes).map{[[id:"candidate_genes"], it]}.collect() : Channel.value([[id:"empty"], []])
                                             ^^^^^^^
  ```

- Warning: `subworkflows/local/annotate_sniffles/main.nf:17:107`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_candidate_genes = candidate_genes ? Channel.fromPath(candidate_genes).map{[[id:"candidate_genes"], it]}.collect() : Channel.value([[id:"empty"], []])
                                                                                                            ^^
  ```

- Warning: `subworkflows/local/annotate_sniffles/main.nf:17:124`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_candidate_genes = candidate_genes ? Channel.fromPath(candidate_genes).map{[[id:"candidate_genes"], it]}.collect() : Channel.value([[id:"empty"], []])
                                                                                                                             ^^^^^^^
  ```

- Warning: `subworkflows/local/annotate_sniffles/main.nf:18:50`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_false_positive_snv = false_positive_snv ? Channel.fromPath(false_positive_snv).map{[[id:"false_positive"], it]}.collect() : Channel.value([[id:"empty"], []])
                                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/annotate_sniffles/main.nf:18:115`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_false_positive_snv = false_positive_snv ? Channel.fromPath(false_positive_snv).map{[[id:"false_positive"], it]}.collect() : Channel.value([[id:"empty"], []])
                                                                                                                    ^^
  ```

- Warning: `subworkflows/local/annotate_sniffles/main.nf:18:132`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_false_positive_snv = false_positive_snv ? Channel.fromPath(false_positive_snv).map{[[id:"false_positive"], it]}.collect() : Channel.value([[id:"empty"], []])
                                                                                                                                     ^^^^^^^
  ```

- Warning: `subworkflows/local/annotate_sniffles/main.nf:19:46`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gene_transcripts = gene_transcripts ? Channel.fromPath(gene_transcripts).map{[[id:"transcripts"], it]}.collect() : Channel.value([[id:"empty"], []])
                                               ^^^^^^^
  ```

- Warning: `subworkflows/local/annotate_sniffles/main.nf:19:106`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_gene_transcripts = gene_transcripts ? Channel.fromPath(gene_transcripts).map{[[id:"transcripts"], it]}.collect() : Channel.value([[id:"empty"], []])
                                                                                                           ^^
  ```

- Warning: `subworkflows/local/annotate_sniffles/main.nf:19:123`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gene_transcripts = gene_transcripts ? Channel.fromPath(gene_transcripts).map{[[id:"transcripts"], it]}.collect() : Channel.value([[id:"empty"], []])
                                                                                                                            ^^^^^^^
  ```

- Warning: `subworkflows/local/annotate_sniffles/main.nf:29:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { id, meta, sv_vcf, hpo ->
                 ^^
  ```

- Warning: `subworkflows/local/annotate_sniffles/main.nf:41:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { id, meta, sv_vcf, snv_vcf ->
                 ^^
  ```

- Warning: `subworkflows/local/annotate_snv/main.nf:15:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, vcf -> [meta, snpeff_db] }.first()
                       ^^^
  ```

- Warning: `subworkflows/local/annotate_snv/main.nf:23:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .combine(SNPEFF_DOWNLOAD.out.cache.map { meta, cache -> cache })
                                                   ^^^^
  ```

- Warning: `subworkflows/local/annotate_snv/main.nf:28:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_vcf_with_cache.map { meta, vcf, meta2, cache -> [meta, vcf] },
                                             ^^^^^
  ```

- Warning: `subworkflows/local/annotate_snv/main.nf:28:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_vcf_with_cache.map { meta, vcf, meta2, cache -> [meta, vcf] },
                                                    ^^^^^
  ```

- Warning: `subworkflows/local/annotate_snv/main.nf:30:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_vcf_with_cache.map { meta, vcf, meta2, cache -> [meta2, cache] }
                                  ^^^^
  ```

- Warning: `subworkflows/local/annotate_snv/main.nf:30:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_vcf_with_cache.map { meta, vcf, meta2, cache -> [meta2, cache] }
                                        ^^^
  ```

- Warning: `subworkflows/local/annotate_svim/main.nf:17:44`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_candidate_genes = candidate_genes ? Channel.fromPath(candidate_genes).map{[[id:"candidate_genes"], it]}.collect() : Channel.value([[id:"empty"], []])
                                             ^^^^^^^
  ```

- Warning: `subworkflows/local/annotate_svim/main.nf:17:107`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_candidate_genes = candidate_genes ? Channel.fromPath(candidate_genes).map{[[id:"candidate_genes"], it]}.collect() : Channel.value([[id:"empty"], []])
                                                                                                            ^^
  ```

- Warning: `subworkflows/local/annotate_svim/main.nf:17:124`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_candidate_genes = candidate_genes ? Channel.fromPath(candidate_genes).map{[[id:"candidate_genes"], it]}.collect() : Channel.value([[id:"empty"], []])
                                                                                                                             ^^^^^^^
  ```

- Warning: `subworkflows/local/annotate_svim/main.nf:18:50`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_false_positive_snv = false_positive_snv ? Channel.fromPath(false_positive_snv).map{[[id:"false_positive"], it]}.collect() : Channel.value([[id:"empty"], []])
                                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/annotate_svim/main.nf:18:115`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_false_positive_snv = false_positive_snv ? Channel.fromPath(false_positive_snv).map{[[id:"false_positive"], it]}.collect() : Channel.value([[id:"empty"], []])
                                                                                                                    ^^
  ```

- Warning: `subworkflows/local/annotate_svim/main.nf:18:132`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_false_positive_snv = false_positive_snv ? Channel.fromPath(false_positive_snv).map{[[id:"false_positive"], it]}.collect() : Channel.value([[id:"empty"], []])
                                                                                                                                     ^^^^^^^
  ```

- Warning: `subworkflows/local/annotate_svim/main.nf:19:46`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gene_transcripts = gene_transcripts ? Channel.fromPath(gene_transcripts).map{[[id:"transcripts"], it]}.collect() : Channel.value([[id:"empty"], []])
                                               ^^^^^^^
  ```

- Warning: `subworkflows/local/annotate_svim/main.nf:19:106`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_gene_transcripts = gene_transcripts ? Channel.fromPath(gene_transcripts).map{[[id:"transcripts"], it]}.collect() : Channel.value([[id:"empty"], []])
                                                                                                           ^^
  ```

- Warning: `subworkflows/local/annotate_svim/main.nf:19:123`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gene_transcripts = gene_transcripts ? Channel.fromPath(gene_transcripts).map{[[id:"transcripts"], it]}.collect() : Channel.value([[id:"empty"], []])
                                                                                                                            ^^^^^^^
  ```

- Warning: `subworkflows/local/annotate_svim/main.nf:29:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { id, meta, sv_vcf, hpo ->
                 ^^
  ```

- Warning: `subworkflows/local/annotate_svim/main.nf:41:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { id, meta, sv_vcf, snv_vcf ->
                 ^^
  ```

- Warning: `subworkflows/local/annotate_unified/main.nf:15:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, vcf -> [meta, snpeff_db] }.first()
                       ^^^
  ```

- Warning: `subworkflows/local/annotate_unified/main.nf:23:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .combine(SNPEFF_DOWNLOAD_UNIFIED.out.cache.map { meta, cache -> cache })
                                                           ^^^^
  ```

- Warning: `subworkflows/local/annotate_unified/main.nf:28:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_vcf_with_cache.map { meta, vcf, meta2, cache -> [meta, vcf] },
                                             ^^^^^
  ```

- Warning: `subworkflows/local/annotate_unified/main.nf:28:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_vcf_with_cache.map { meta, vcf, meta2, cache -> [meta, vcf] },
                                                    ^^^^^
  ```

- Warning: `subworkflows/local/annotate_unified/main.nf:30:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_vcf_with_cache.map { meta, vcf, meta2, cache -> [meta2, cache] }
                                  ^^^^
  ```

- Warning: `subworkflows/local/annotate_unified/main.nf:30:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_vcf_with_cache.map { meta, vcf, meta2, cache -> [meta2, cache] }
                                        ^^^
  ```

- Warning: `subworkflows/local/annotsv_db/main.nf:14:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { [[id:"annotsv"], it] }
                                      ^^
  ```

- Warning: `subworkflows/local/annotsv_db/main.nf:18:40`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_annotsv_annotations_input = Channel.fromPath(annotsv_annotations).map{[[id:"annotsv_annotations"], it]}.collect()
                                         ^^^^^^^
  ```

- Warning: `subworkflows/local/annotsv_db/main.nf:18:111`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_annotsv_annotations_input = Channel.fromPath(annotsv_annotations).map{[[id:"annotsv_annotations"], it]}.collect()
                                                                                                                ^^
  ```

- Warning: `subworkflows/local/annotsv_db/main.nf:25:38`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_annotsv_annotations = Channel.fromPath(annotsv_annotations).map{[[id:"annotsv_annotations"], it]}.collect()
                                       ^^^^^^^
  ```

- Warning: `subworkflows/local/annotsv_db/main.nf:25:109`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_annotsv_annotations = Channel.fromPath(annotsv_annotations).map{[[id:"annotsv_annotations"], it]}.collect()
                                                                                                              ^^
  ```

- Warning: `subworkflows/local/bam2fastq/main.nf:15:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/call_hificnv/main.nf:12:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv/main.nf:19:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv/main.nf:21:14`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_vcf = Channel.empty()
               ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv/main.nf:22:14`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_tbi = Channel.empty()
               ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv/main.nf:23:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gvcf = Channel.empty()
                ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv/main.nf:24:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gtbi = Channel.empty()
                ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv/main.nf:25:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_vcf_deepvariant = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv/main.nf:26:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_tbi_deepvariant = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv/main.nf:27:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      html_report = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv/main.nf:76:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              Channel.value([]),   // empty channel for samples
              ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv/main.nf:77:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              Channel.value([]),   // empty channel for regions
              ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv/main.nf:78:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              Channel.value([])    // empty channel for filters
              ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv/main.nf:109:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  Channel.value([]),
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv/main.nf:110:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  Channel.value([]),
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv/main.nf:111:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  Channel.value([])
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv/main.nf:129:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              html_report = Channel.empty()  // FIXED: Added parentheses
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/call_str/main.nf:14:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/call_sv/main.nf:82:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, vcf, tbi -> vcf != null }
                    ^^^^
  ```

- Warning: `subworkflows/local/call_sv/main.nf:82:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, vcf, tbi -> vcf != null }
                               ^^^
  ```

- Warning: `subworkflows/local/call_sv/main.nf:85:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, vcf, tbi -> vcf != null }
                    ^^^^
  ```

- Warning: `subworkflows/local/call_sv/main.nf:85:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, vcf, tbi -> vcf != null }
                               ^^^
  ```

- Warning: `subworkflows/local/filter_sv/main.nf:20:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  ch_versions = Channel.empty()
                ^^^^^^^
  ```

- Warning: `subworkflows/local/filter_sv/main.nf:21:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  target_bed_ch = target_bed ?: Channel.value([])
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/filter_sv/main.nf:26:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.value([]),
      ^^^^^^^
  ```

- Warning: `subworkflows/local/filter_sv/main.nf:28:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.value([])
      ^^^^^^^
  ```

- Warning: `subworkflows/local/filter_sv/main.nf:48:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { clean_meta, vcf, tbi, original_meta, summary, bed ->
                     ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/filter_sv/main.nf:53:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_sv_mosdepth_bed.map { meta, vcf, tbi, summary, bed -> tuple(meta, vcf, tbi) },
                                                       ^^^^^^^
  ```

- Warning: `subworkflows/local/filter_sv/main.nf:53:63`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_sv_mosdepth_bed.map { meta, vcf, tbi, summary, bed -> tuple(meta, vcf, tbi) },
                                                                ^^^
  ```

- Warning: `subworkflows/local/filter_sv/main.nf:54:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_sv_mosdepth_bed.map { meta, vcf, tbi, summary, bed -> tuple(meta, summary) },
                                             ^^^
  ```

- Warning: `subworkflows/local/filter_sv/main.nf:54:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_sv_mosdepth_bed.map { meta, vcf, tbi, summary, bed -> tuple(meta, summary) },
                                                  ^^^
  ```

- Warning: `subworkflows/local/filter_sv/main.nf:54:63`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_sv_mosdepth_bed.map { meta, vcf, tbi, summary, bed -> tuple(meta, summary) },
                                                                ^^^
  ```

- Warning: `subworkflows/local/filter_sv/main.nf:55:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_sv_mosdepth_bed.map { meta, vcf, tbi, summary, bed -> tuple(meta, bed) },
                                             ^^^
  ```

- Warning: `subworkflows/local/filter_sv/main.nf:55:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_sv_mosdepth_bed.map { meta, vcf, tbi, summary, bed -> tuple(meta, bed) },
                                                  ^^^
  ```

- Warning: `subworkflows/local/filter_sv/main.nf:55:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_sv_mosdepth_bed.map { meta, vcf, tbi, summary, bed -> tuple(meta, bed) },
                                                       ^^^^^^^
  ```

- Warning: `subworkflows/local/haplotag_bam/main.nf:13:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/joint_genotype_snv/main.nf:13:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/joint_genotype_snv/main.nf:17:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, data -> [data.id, data.family_id] }
                 ^^^^
  ```

- Warning: `subworkflows/local/joint_genotype_snv/main.nf:18:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { sample_id, family_id ->
                    ^^^^^^^^^
  ```

- Warning: `subworkflows/local/joint_genotype_snv/main.nf:26:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { sample_id, gvcf, family_id -> [family_id, gvcf] }
                 ^^^^^^^^^
  ```

- Warning: `subworkflows/local/joint_genotype_snv/main.nf:28:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { family_id, gvcfs -> gvcfs.size() == 3 }  // Only trios
                    ^^^^^^^^^
  ```

- Warning: `subworkflows/local/longphase_variants/main.nf:13:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/merge_sv/main.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/merge_sv/main.nf:23:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_chr_norm ?: Channel.value([])
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/merge_sv/main.nf:32:76`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      jasmine_vcf = FIX_HEADER_JASMINE.out.vcf_with_samples.map { meta, vcf, samples -> [meta, vcf] }
                                                                             ^^^^^^^
  ```

- Warning: `subworkflows/local/merge_sv/main.nf:39:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.value([]),  // regions - use Channel.value([]) instead of []
          ^^^^^^^
  ```

- Warning: `subworkflows/local/merge_sv/main.nf:40:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.value([]),  // targets
          ^^^^^^^
  ```

- Warning: `subworkflows/local/merge_sv/main.nf:41:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.value([])   // samples
          ^^^^^^^
  ```

- Warning: `subworkflows/local/merge_sv/main.nf:49:69`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  FIX_HEADER_JASMINE.out.vcf_with_samples.map { meta, vcf, samples -> [meta, samples] },
                                                                      ^^^
  ```

- Warning: `subworkflows/local/methyl/main.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/mosdepth/main.nf:15:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/rtg_compare_snv/main.nf:13:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/rtg_compare_sv/main.nf:14:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/sniffles_trio/main.nf:16:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              samplesheet.map { meta, data -> [data.id, data.family_id] },
                                ^^^^
  ```

- Warning: `subworkflows/local/sniffles_trio/main.nf:19:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { sample_id, snf, family_id ->
                    ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sniffles_trio/main.nf:19:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { sample_id, snf, family_id ->
                               ^^^
  ```

- Warning: `subworkflows/local/sniffles_trio/main.nf:22:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { sample_id, snf, family_id -> [family_id, snf] }  // Key by family_id
                 ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sniffles_trio/main.nf:24:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { family_id, snf_files_list -> snf_files_list.size() == 3 }
                    ^^^^^^^^^
  ```

- Warning: `subworkflows/local/unify_vcf/main.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_longraredisease_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs (FIXED: removed underscore)
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_longraredisease_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet (FIXED: removed underscore)
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_longraredisease_pipeline/main.nf:42:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_longraredisease_pipeline/main.nf:166:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_samplesheet = Channel.fromList(samplesheet_data)
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_longraredisease_pipeline/main.nf:364:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def baseTools = Channel.from(['nextflow', 'nf_core', 'bioconda', 'biocontainers', 'multiqc'])
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_longraredisease_pipeline/main.nf:393:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          paramsMap.each { param, paramStatus ->
                                  ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_longraredisease_pipeline/main.nf:423:61`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def dependentWorkflows = workflowDependencies.findAll { workflow, dependencies ->
                                                              ^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_longraredisease_pipeline/main.nf:427:41`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      dependentWorkflows.each { workflow, dependencies ->
                                          ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_longraredisease_pipeline/main.nf:443:61`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          def requiringWorkflows = fileDependencies.findAll { workflow, files ->
                                                              ^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_longraredisease_pipeline/main.nf:447:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          requiringWorkflows.each { workflow, files ->
                                              ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_longraredisease_pipeline/main.nf:460:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      return param ? Channel.fromPath(param, checkIfExists: true)
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_longraredisease_pipeline/main.nf:467:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      return param ? Channel.fromList(samplesheetToList(param, schema)) : defaultValue
                     ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_stats_samtools/main.nf:15:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/longraredisease.nf:102:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_samplesheet = Channel.fromList(samplesheet_data)
                       ^^^^^^^
  ```

- Warning: `workflows/longraredisease.nf:128:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, data ->
                 ^^^^
  ```

- Warning: `workflows/longraredisease.nf:148:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/longraredisease.nf:150:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_fasta = Channel
                 ^^^^^^^
  ```

- Warning: `workflows/longraredisease.nf:175:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, data -> data.family_id }
                     ^^^^
  ```

- Warning: `workflows/longraredisease.nf:180:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, sdf -> sdf }  // Extract just the SDF path
                     ^^^^
  ```

- Warning: `workflows/longraredisease.nf:190:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_trf = Channel
                   ^^^^^^^
  ```

- Warning: `workflows/longraredisease.nf:199:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ch_trf = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `workflows/longraredisease.nf:226:21`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      it.name.endsWith('.fastq.gz') || it.name.endsWith('.fq.gz')
                      ^^
  ```

- Warning: `workflows/longraredisease.nf:226:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      it.name.endsWith('.fastq.gz') || it.name.endsWith('.fq.gz')
                                                       ^^
  ```

- Warning: `workflows/longraredisease.nf:299:68`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      def bam_files = bam_path.listFiles().findAll { it.name.endsWith('.bam') }
                                                                     ^^
  ```

- Warning: `workflows/longraredisease.nf:366:65`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_final_sorted_bam = ch_aligned_input.map { meta, bam, bai -> [meta, bam] }
                                                                  ^^^
  ```

- Warning: `workflows/longraredisease.nf:367:60`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_final_sorted_bai = ch_aligned_input.map { meta, bam, bai -> [meta, bai] }
                                                             ^^^
  ```

- Warning: `workflows/longraredisease.nf:566:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      .filter { meta, vcf, tbi -> vcf != null }
                                ^^^^
  ```

- Warning: `workflows/longraredisease.nf:566:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      .filter { meta, vcf, tbi -> vcf != null }
                                           ^^^
  ```

- Warning: `workflows/longraredisease.nf:576:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_sv_vcf_final = FILTER_SV_SNIFFLES.out.ch_vcf_tbi.map { meta, vcf, tbi -> [meta, vcf] }
                                                                                   ^^^
  ```

- Warning: `workflows/longraredisease.nf:584:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .filter { meta, vcf, tbi -> vcf != null }
                            ^^^^
  ```

- Warning: `workflows/longraredisease.nf:584:38`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .filter { meta, vcf, tbi -> vcf != null }
                                       ^^^
  ```

- Warning: `workflows/longraredisease.nf:595:74`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_svim_vcf = FILTER_SV_SVIM.out.ch_vcf_tbi.map { meta, vcf, tbi -> [meta, vcf] }
                                                                           ^^^
  ```

- Warning: `workflows/longraredisease.nf:601:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_sv_vcf_final = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `workflows/longraredisease.nf:655:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, data ->
                    ^^^^
  ```

- Warning: `workflows/longraredisease.nf:670:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { sample_id, meta, vcf, hpo_terms ->
                 ^^^^^^^^^
  ```

- Warning: `workflows/longraredisease.nf:677:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_sv_svanna.map { meta, vcf, hpo_terms -> [meta, vcf] },
                                            ^^^^^^^^^
  ```

- Warning: `workflows/longraredisease.nf:679:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_sv_svanna.map { meta, vcf, hpo_terms -> hpo_terms }
                                 ^^^^
  ```

- Warning: `workflows/longraredisease.nf:679:38`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_sv_svanna.map { meta, vcf, hpo_terms -> hpo_terms }
                                       ^^^
  ```

- Warning: `workflows/longraredisease.nf:764:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_str_vcf = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `workflows/longraredisease.nf:803:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_cnv_vcf = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `workflows/longraredisease.nf:852:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_cnv_vcf = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `workflows/longraredisease.nf:868:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .filter { meta, vcf, tbi -> vcf != null }
                            ^^^^
  ```

- Warning: `workflows/longraredisease.nf:868:38`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .filter { meta, vcf, tbi -> vcf != null }
                                       ^^^
  ```

- Warning: `workflows/longraredisease.nf:879:78`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_cutesv_vcf = FILTER_SV_CUTESV.out.ch_vcf_tbi.map { meta, vcf, tbi -> [meta, vcf] }
                                                                               ^^^
  ```

- Warning: `workflows/longraredisease.nf:943:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_combined.map { meta, sv, cnv, str -> [meta, sv] },
                                      ^^^
  ```

- Warning: `workflows/longraredisease.nf:943:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_combined.map { meta, sv, cnv, str -> [meta, sv] },
                                           ^^^
  ```

- Warning: `workflows/longraredisease.nf:944:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_combined.map { meta, sv, cnv, str -> [meta, cnv ?: []] },
                                  ^^
  ```

- Warning: `workflows/longraredisease.nf:944:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_combined.map { meta, sv, cnv, str -> [meta, cnv ?: []] },
                                           ^^^
  ```

- Warning: `workflows/longraredisease.nf:945:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_combined.map { meta, sv, cnv, str -> [meta, str ?: []] },
                                  ^^
  ```

- Warning: `workflows/longraredisease.nf:945:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_combined.map { meta, sv, cnv, str -> [meta, str ?: []] },
                                      ^^^
  ```
