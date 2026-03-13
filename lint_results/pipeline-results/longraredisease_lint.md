# Nextflow lint results

- Generated: 2026-03-13T00:20:46.369640670Z
- Nextflow version: 26.02.0-edge
- Summary: 7 errors, 135 warnings

## :x: Errors

- Error: `nextflow.config:381:39`: `manifest` is not defined

  ```nextflow
  \033[0;35m  nf-core/longraredisease ${manifest.version}\033[0m
                                        ^^^^^^^^
  ```

- Error: `nextflow.config:384:26`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                           ^^^^^^^^
  ```

- Error: `nextflow.config:384:69`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                      ^^^^^^^^
  ```

- Error: `nextflow.config:384:186`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                                                                                                                                           ^^^^^^^^
  ```

- Error: `nextflow.config:393:22`: `validation` is not defined

  ```nextflow
          beforeText = validation.help.beforeText
                       ^^^^^^^^^^
  ```

- Error: `nextflow.config:394:21`: `validation` is not defined

  ```nextflow
          afterText = validation.help.afterText
                      ^^^^^^^^^^
  ```

- Error: `subworkflows/local/align.nf:80:9`: Incorrect number of call arguments, expected 4 but received 3

  ```nextflow
          SAMTOOLS_VIEW(
          ^
  ```

## :warning: Warnings

- Warning: `conf/modules.config:467:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          return args_list.findAll { it }.join(' ').trim()
                                     ^^
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

- Warning: `modules/local/sniffles/generate_plots/main.nf:43:9`: Variable was declared but not used

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

- Warning: `nextflow.config:384:129`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                                                                                  ^^
  ```

- Warning: `subworkflows/local/align.nf:17:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/align.nf:42:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta_sample, reads, meta_ref, index ->
                                         ^^^^^^^^
  ```

- Warning: `subworkflows/local/align.nf:54:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_align_input.map { meta_sample, reads, meta_index, index ->
                                                       ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/align.nf:54:66`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_align_input.map { meta_sample, reads, meta_index, index ->
                                                                   ^^^^^
  ```

- Warning: `subworkflows/local/align.nf:57:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_align_input.map { meta_sample, reads, meta_index, index ->
                                   ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/align.nf:57:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_align_input.map { meta_sample, reads, meta_index, index ->
                                                ^^^^^
  ```

- Warning: `subworkflows/local/annotate_sv.nf:17:44`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_candidate_genes = candidate_genes ? Channel.fromPath(candidate_genes).map{[[id:"candidate_genes"], it]}.collect() : Channel.value([[id:"empty"], []])
                                             ^^^^^^^
  ```

- Warning: `subworkflows/local/annotate_sv.nf:17:107`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_candidate_genes = candidate_genes ? Channel.fromPath(candidate_genes).map{[[id:"candidate_genes"], it]}.collect() : Channel.value([[id:"empty"], []])
                                                                                                            ^^
  ```

- Warning: `subworkflows/local/annotate_sv.nf:17:124`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_candidate_genes = candidate_genes ? Channel.fromPath(candidate_genes).map{[[id:"candidate_genes"], it]}.collect() : Channel.value([[id:"empty"], []])
                                                                                                                             ^^^^^^^
  ```

- Warning: `subworkflows/local/annotate_sv.nf:18:50`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_false_positive_snv = false_positive_snv ? Channel.fromPath(false_positive_snv).map{[[id:"false_positive"], it]}.collect() : Channel.value([[id:"empty"], []])
                                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/annotate_sv.nf:18:115`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_false_positive_snv = false_positive_snv ? Channel.fromPath(false_positive_snv).map{[[id:"false_positive"], it]}.collect() : Channel.value([[id:"empty"], []])
                                                                                                                    ^^
  ```

- Warning: `subworkflows/local/annotate_sv.nf:18:132`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_false_positive_snv = false_positive_snv ? Channel.fromPath(false_positive_snv).map{[[id:"false_positive"], it]}.collect() : Channel.value([[id:"empty"], []])
                                                                                                                                     ^^^^^^^
  ```

- Warning: `subworkflows/local/annotate_sv.nf:19:46`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gene_transcripts = gene_transcripts ? Channel.fromPath(gene_transcripts).map{[[id:"transcripts"], it]}.collect() : Channel.value([[id:"empty"], []])
                                               ^^^^^^^
  ```

- Warning: `subworkflows/local/annotate_sv.nf:19:106`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_gene_transcripts = gene_transcripts ? Channel.fromPath(gene_transcripts).map{[[id:"transcripts"], it]}.collect() : Channel.value([[id:"empty"], []])
                                                                                                           ^^
  ```

- Warning: `subworkflows/local/annotate_sv.nf:19:123`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gene_transcripts = gene_transcripts ? Channel.fromPath(gene_transcripts).map{[[id:"transcripts"], it]}.collect() : Channel.value([[id:"empty"], []])
                                                                                                                            ^^^^^^^
  ```

- Warning: `subworkflows/local/annotate_sv.nf:29:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { id, meta, sv_vcf, hpo ->
                 ^^
  ```

- Warning: `subworkflows/local/annotate_sv.nf:41:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { id, meta, sv_vcf, snv_vcf ->
                 ^^
  ```

- Warning: `subworkflows/local/annotsv_db.nf:14:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { [[id:"annotsv"], it] }
                                      ^^
  ```

- Warning: `subworkflows/local/annotsv_db.nf:18:40`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_annotsv_annotations_input = Channel.fromPath(annotsv_annotations).map{[[id:"annotsv_annotations"], it]}.collect()
                                         ^^^^^^^
  ```

- Warning: `subworkflows/local/annotsv_db.nf:18:111`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_annotsv_annotations_input = Channel.fromPath(annotsv_annotations).map{[[id:"annotsv_annotations"], it]}.collect()
                                                                                                                ^^
  ```

- Warning: `subworkflows/local/annotsv_db.nf:25:38`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_annotsv_annotations = Channel.fromPath(annotsv_annotations).map{[[id:"annotsv_annotations"], it]}.collect()
                                       ^^^^^^^
  ```

- Warning: `subworkflows/local/annotsv_db.nf:25:109`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_annotsv_annotations = Channel.fromPath(annotsv_annotations).map{[[id:"annotsv_annotations"], it]}.collect()
                                                                                                              ^^
  ```

- Warning: `subworkflows/local/bam2fastq.nf:15:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/call_hificnv.nf:12:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv.nf:19:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv.nf:21:14`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_vcf = Channel.empty()
               ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv.nf:22:14`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_tbi = Channel.empty()
               ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv.nf:23:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gvcf = Channel.empty()
                ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv.nf:24:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gtbi = Channel.empty()
                ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv.nf:74:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              Channel.value([]),   // empty channel for samples
              ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv.nf:75:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              Channel.value([]),   // empty channel for regions
              ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv.nf:76:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              Channel.value([])    // empty channel for filters
              ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv.nf:110:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  Channel.value([]),
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv.nf:111:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  Channel.value([]),
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv.nf:112:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  Channel.value([])
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv.nf:140:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_vcf_deepvariant = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv.nf:141:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_tbi_deepvariant = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `subworkflows/local/call_str.nf:14:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/call_sv.nf:79:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, vcf, tbi -> vcf != null }
                    ^^^^
  ```

- Warning: `subworkflows/local/call_sv.nf:79:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, vcf, tbi -> vcf != null }
                               ^^^
  ```

- Warning: `subworkflows/local/call_sv.nf:82:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, vcf, tbi -> vcf != null }
                    ^^^^
  ```

- Warning: `subworkflows/local/call_sv.nf:82:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, vcf, tbi -> vcf != null }
                               ^^^
  ```

- Warning: `subworkflows/local/filter_sv.nf:20:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  ch_versions = Channel.empty()
                ^^^^^^^
  ```

- Warning: `subworkflows/local/filter_sv.nf:21:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  target_bed_ch = target_bed ?: Channel.value([])
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/filter_sv.nf:26:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.value([]),
      ^^^^^^^
  ```

- Warning: `subworkflows/local/filter_sv.nf:28:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.value([])
      ^^^^^^^
  ```

- Warning: `subworkflows/local/filter_sv.nf:48:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { clean_meta, vcf, tbi, original_meta, summary, bed ->
                     ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/filter_sv.nf:53:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_sv_mosdepth_bed.map { meta, vcf, tbi, summary, bed -> tuple(meta, vcf, tbi) },
                                                       ^^^^^^^
  ```

- Warning: `subworkflows/local/filter_sv.nf:53:63`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_sv_mosdepth_bed.map { meta, vcf, tbi, summary, bed -> tuple(meta, vcf, tbi) },
                                                                ^^^
  ```

- Warning: `subworkflows/local/filter_sv.nf:54:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_sv_mosdepth_bed.map { meta, vcf, tbi, summary, bed -> tuple(meta, summary) },
                                             ^^^
  ```

- Warning: `subworkflows/local/filter_sv.nf:54:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_sv_mosdepth_bed.map { meta, vcf, tbi, summary, bed -> tuple(meta, summary) },
                                                  ^^^
  ```

- Warning: `subworkflows/local/filter_sv.nf:54:63`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_sv_mosdepth_bed.map { meta, vcf, tbi, summary, bed -> tuple(meta, summary) },
                                                                ^^^
  ```

- Warning: `subworkflows/local/filter_sv.nf:55:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_sv_mosdepth_bed.map { meta, vcf, tbi, summary, bed -> tuple(meta, bed) },
                                             ^^^
  ```

- Warning: `subworkflows/local/filter_sv.nf:55:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_sv_mosdepth_bed.map { meta, vcf, tbi, summary, bed -> tuple(meta, bed) },
                                                  ^^^
  ```

- Warning: `subworkflows/local/filter_sv.nf:55:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_sv_mosdepth_bed.map { meta, vcf, tbi, summary, bed -> tuple(meta, bed) },
                                                       ^^^^^^^
  ```

- Warning: `subworkflows/local/haplotag_bam.nf:13:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/joint_genotype_snv.nf:13:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/joint_genotype_snv.nf:17:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, data -> [data.id, data.family_id] }
                 ^^^^
  ```

- Warning: `subworkflows/local/joint_genotype_snv.nf:18:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { sample_id, family_id ->
                    ^^^^^^^^^
  ```

- Warning: `subworkflows/local/joint_genotype_snv.nf:26:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { sample_id, gvcf, family_id -> [family_id, gvcf] }
                 ^^^^^^^^^
  ```

- Warning: `subworkflows/local/joint_genotype_snv.nf:28:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { family_id, gvcfs -> gvcfs.size() == 3 }  // Only trios
                    ^^^^^^^^^
  ```

- Warning: `subworkflows/local/longphase_variants.nf:13:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/merge_sv.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/merge_sv.nf:23:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_chr_norm ?: Channel.value([])
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/merge_sv.nf:32:76`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      jasmine_vcf = FIX_HEADER_JASMINE.out.vcf_with_samples.map { meta, vcf, samples -> [meta, vcf] }
                                                                             ^^^^^^^
  ```

- Warning: `subworkflows/local/merge_sv.nf:39:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.value([]),  // regions - use Channel.value([]) instead of []
          ^^^^^^^
  ```

- Warning: `subworkflows/local/merge_sv.nf:40:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.value([]),  // targets
          ^^^^^^^
  ```

- Warning: `subworkflows/local/merge_sv.nf:41:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.value([])   // samples
          ^^^^^^^
  ```

- Warning: `subworkflows/local/merge_sv.nf:49:69`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  FIX_HEADER_JASMINE.out.vcf_with_samples.map { meta, vcf, samples -> [meta, samples] },
                                                                      ^^^
  ```

- Warning: `subworkflows/local/methyl.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/mosdepth.nf:15:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/rtg_compare_snv.nf:13:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/rtg_compare_sv.nf:14:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/sniffles_trio.nf:16:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              samplesheet.map { meta, data -> [data.id, data.family_id] },
                                ^^^^
  ```

- Warning: `subworkflows/local/sniffles_trio.nf:19:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { sample_id, snf, family_id ->
                    ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sniffles_trio.nf:19:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { sample_id, snf, family_id ->
                               ^^^
  ```

- Warning: `subworkflows/local/sniffles_trio.nf:22:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { sample_id, snf, family_id -> [family_id, snf] }  // Key by family_id
                 ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sniffles_trio.nf:24:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { family_id, snf_files_list -> snf_files_list.size() == 3 }
                    ^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_longraredisease_pipeline/main.nf:31:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_longraredisease_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_longraredisease_pipeline/main.nf:38:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_longraredisease_pipeline/main.nf:75:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_stats_samtools/main.nf:15:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:101:98`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      return ch_versions.unique().map { version -> processVersionsFromYAML(version) }.unique().mix(Channel.of(workflowVersionToYAML()))
                                                                                                   ^^^^^^^
  ```

- Warning: `workflows/longraredisease.nf:96:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_samplesheet = Channel.fromList(samplesheet_data)
                       ^^^^^^^
  ```

- Warning: `workflows/longraredisease.nf:122:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, data ->
                 ^^^^
  ```

- Warning: `workflows/longraredisease.nf:142:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/longraredisease.nf:144:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_fasta = Channel
                 ^^^^^^^
  ```

- Warning: `workflows/longraredisease.nf:169:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, data -> data.family_id }
                     ^^^^
  ```

- Warning: `workflows/longraredisease.nf:174:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, sdf -> sdf }  // Extract just the SDF path
                     ^^^^
  ```

- Warning: `workflows/longraredisease.nf:184:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_trf = Channel
                   ^^^^^^^
  ```

- Warning: `workflows/longraredisease.nf:193:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ch_trf = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `workflows/longraredisease.nf:220:21`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      it.name.endsWith('.fastq.gz') || it.name.endsWith('.fq.gz')
                      ^^
  ```

- Warning: `workflows/longraredisease.nf:220:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      it.name.endsWith('.fastq.gz') || it.name.endsWith('.fq.gz')
                                                       ^^
  ```

- Warning: `workflows/longraredisease.nf:293:68`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      def bam_files = bam_path.listFiles().findAll { it.name.endsWith('.bam') }
                                                                     ^^
  ```

- Warning: `workflows/longraredisease.nf:360:65`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_final_sorted_bam = ch_aligned_input.map { meta, bam, bai -> [meta, bam] }
                                                                  ^^^
  ```

- Warning: `workflows/longraredisease.nf:361:60`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_final_sorted_bai = ch_aligned_input.map { meta, bam, bai -> [meta, bai] }
                                                             ^^^
  ```

- Warning: `workflows/longraredisease.nf:568:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      .filter { meta, vcf, tbi -> vcf != null }
                                ^^^^
  ```

- Warning: `workflows/longraredisease.nf:568:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      .filter { meta, vcf, tbi -> vcf != null }
                                           ^^^
  ```

- Warning: `workflows/longraredisease.nf:578:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_final_sv_vcf = filter_sv_sniffles.out.ch_vcf_tbi.map { meta, vcf, tbi -> [meta, vcf] }
                                                                                   ^^^
  ```

- Warning: `workflows/longraredisease.nf:585:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      .filter { meta, vcf, tbi -> vcf != null }
                                ^^^^
  ```

- Warning: `workflows/longraredisease.nf:585:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      .filter { meta, vcf, tbi -> vcf != null }
                                           ^^^
  ```

- Warning: `workflows/longraredisease.nf:595:74`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_svim_vcf = filter_sv_svim.out.ch_vcf_tbi.map { meta, vcf, tbi -> [meta, vcf] }
                                                                           ^^^
  ```

- Warning: `workflows/longraredisease.nf:602:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      .filter { meta, vcf, tbi -> vcf != null }
                                ^^^^
  ```

- Warning: `workflows/longraredisease.nf:602:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      .filter { meta, vcf, tbi -> vcf != null }
                                           ^^^
  ```

- Warning: `workflows/longraredisease.nf:612:78`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_cutesv_vcf = filter_sv_cutesv.out.ch_vcf_tbi.map { meta, vcf, tbi -> [meta, vcf] }
                                                                               ^^^
  ```

- Warning: `workflows/longraredisease.nf:706:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, data ->
                        ^^^^
  ```

- Warning: `workflows/longraredisease.nf:724:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_svanna_db = Channel
                         ^^^^^^^
  ```

- Warning: `workflows/longraredisease.nf:730:55`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_sv_vcf_for_annotation.map { meta, vcf, hpo_terms -> [meta, vcf] },
                                                        ^^^^^^^^^
  ```

- Warning: `workflows/longraredisease.nf:732:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_sv_vcf_for_annotation.map { meta, vcf, hpo_terms -> hpo_terms }
                                             ^^^^
  ```

- Warning: `workflows/longraredisease.nf:732:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_sv_vcf_for_annotation.map { meta, vcf, hpo_terms -> hpo_terms }
                                                   ^^^
  ```
