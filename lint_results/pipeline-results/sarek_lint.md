# Nextflow lint results

- Generated: 2026-04-21T00:33:07.425221569Z
- Nextflow version: 26.03.3-edge
- Summary: 646 warnings

## :warning: Warnings

- Warning: `conf/modules/aligner.config:51:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      ) { "mapped/${meta.id}/${it}" }
                                               ^^
  ```

- Warning: `conf/modules/aligner.config:81:178`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { (params.save_output_as_bam && (params.save_mapped || params.skip_tools && params.skip_tools.split(',').contains('markduplicates'))) ? "mapped/${meta.id}/${it}" : null }
                                                                                                                                                                                   ^^
  ```

- Warning: `conf/modules/aligner_parabricks.config:31:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_mapped ? it : null }
                                             ^^
  ```

- Warning: `conf/modules/aligner_parabricks.config:41:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_mapped ? it : null }
                                             ^^
  ```

- Warning: `conf/modules/aligner_parabricks.config:50:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_mapped ? it : null }
                                             ^^
  ```

- Warning: `conf/modules/aligner_parabricks.config:60:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_output_as_bam ? it : null }
                                                    ^^
  ```

- Warning: `conf/modules/annotate.config:27:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      saveAs: { params.tools.split(',').contains('snpeff') ? it : null }
                                                                             ^^
  ```

- Warning: `conf/modules/annotate.config:88:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_reference ? it : null }
                                                    ^^
  ```

- Warning: `conf/modules/annotate.config:126:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.tools.split(',').contains('snpeff') ? it : null }
                                                                         ^^
  ```

- Warning: `conf/modules/contamination.config:17:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_bbsplit_reads ? it : null }
                                                        ^^
  ```

- Warning: `conf/modules/deepvariant.config:29:81`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { meta.num_intervals > 1 ? null : "deepvariant/${meta.id}/${it}" }
                                                                                  ^^
  ```

- Warning: `conf/modules/freebayes.config:43:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { meta.num_intervals > 1 ? null : "freebayes/${meta.id}/${it}" }
                                                                                ^^
  ```

- Warning: `conf/modules/haplotypecaller.config:29:85`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { meta.num_intervals > 1 ? null : "haplotypecaller/${meta.id}/${it}" }
                                                                                      ^^
  ```

- Warning: `conf/modules/lofreq.config:26:80`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { meta.num_intervals > 1 ? null : "lofreq/${meta.id}/${it}" }
                                                                                 ^^
  ```

- Warning: `conf/modules/markduplicates.config:32:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { !params.save_output_as_bam ? it : null }
                                                     ^^
  ```

- Warning: `conf/modules/markduplicates.config:59:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { !params.save_output_as_bam ? it : null }
                                                     ^^
  ```

- Warning: `conf/modules/markduplicates.config:88:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { !params.save_output_as_bam ? it : null }
                                                         ^^
  ```

- Warning: `conf/modules/markduplicates.config:94:145`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { !(params.skip_tools && params.skip_tools.split(',').contains('markduplicates_report')) ? "markduplicates/${meta.id}/${it}" : null}
                                                                                                                                                  ^^
  ```

- Warning: `conf/modules/markduplicates.config:107:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { !params.save_output_as_bam ? it : null }
                                                     ^^
  ```

- Warning: `conf/modules/markduplicates.config:116:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { !params.save_output_as_bam ? it : null }
                                                     ^^
  ```

- Warning: `conf/modules/markduplicates.config:130:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_output_as_bam ? it : null }
                                                        ^^
  ```

- Warning: `conf/modules/markduplicates.config:136:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_output_as_bam ? it : null }
                                                        ^^
  ```

- Warning: `conf/modules/mpileup.config:33:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { meta.num_intervals > 1 ? null : it }
                                                        ^^
  ```

- Warning: `conf/modules/mutect2.config:26:81`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { meta.num_intervals > 1 ? null : "mutect2/${meta.id}/${it}" }
                                                                                  ^^
  ```

- Warning: `conf/modules/mutect2.config:98:81`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { meta.num_intervals > 1 ? null : "mutect2/${meta.id}/${it}" }
                                                                                  ^^
  ```

- Warning: `conf/modules/prepare_genome.config:21:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:31:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:40:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:50:84`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? "cnvkit/${it}" : null }
                                                                                     ^^
  ```

- Warning: `conf/modules/prepare_genome.config:61:84`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? "cnvkit/${it}" : null }
                                                                                     ^^
  ```

- Warning: `conf/modules/prepare_genome.config:70:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:79:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:88:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:97:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:106:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:115:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:124:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:133:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:142:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:151:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:160:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:175:78`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { (params.save_reference || params.build_only_index) && !it.equals('versions.yml') ? it : null }
                                                                               ^^
  ```

- Warning: `conf/modules/prepare_genome.config:175:106`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { (params.save_reference || params.build_only_index) && !it.equals('versions.yml') ? it : null }
                                                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:186:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_intervals.config:28:87`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? "intervals/${it}" : null }
                                                                                        ^^
  ```

- Warning: `conf/modules/prepare_intervals.config:37:87`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? "intervals/${it}" : null }
                                                                                        ^^
  ```

- Warning: `conf/modules/prepare_intervals.config:47:87`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? "intervals/${it}" : null }
                                                                                        ^^
  ```

- Warning: `conf/modules/prepare_recalibration.config:25:81`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { meta.num_intervals > 1 ? null : "recal_table/${meta.id}/${it}" }
                                                                                  ^^
  ```

- Warning: `conf/modules/recalibrate.config:28:111`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { !params.save_output_as_bam ? meta.num_intervals > 1 ? null : "recalibrated/${meta.id}/${it}" : null }
                                                                                                                ^^
  ```

- Warning: `conf/modules/recalibrate.config:34:110`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_output_as_bam ? meta.num_intervals > 1 ? null : "recalibrated/${meta.id}/${it}" : null }
                                                                                                               ^^
  ```

- Warning: `conf/modules/recalibrate.config:40:110`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_output_as_bam ? meta.num_intervals > 1 ? null : "recalibrated/${meta.id}/${it.replace('.bai', '.bam.bai')}" : null }
                                                                                                               ^^
  ```

- Warning: `conf/modules/recalibrate.config:51:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { !params.save_output_as_bam ? it : null }
                                                         ^^
  ```

- Warning: `conf/modules/recalibrate.config:60:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { !params.save_output_as_bam ? it : null }
                                                         ^^
  ```

- Warning: `conf/modules/recalibrate.config:71:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_output_as_bam ? it : null }
                                                    ^^
  ```

- Warning: `conf/modules/sentieon_dedup.config:32:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { !params.save_output_as_bam ? it : null }
                                                         ^^
  ```

- Warning: `conf/modules/sentieon_dedup.config:38:145`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { !(params.skip_tools && params.skip_tools.split(',').contains('sentieon_dedup_report')) ? "sentieon_dedup/${meta.id}/${it}" : null}
                                                                                                                                                  ^^
  ```

- Warning: `conf/modules/sentieon_dnascope.config:25:87`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { meta.num_intervals > 1 ? null : "sentieon_dnascope/${meta.id}/${it}" }
                                                                                        ^^
  ```

- Warning: `conf/modules/sentieon_haplotyper.config:25:89`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { meta.num_intervals > 1 ? null : "sentieon_haplotyper/${meta.id}/${it}" }
                                                                                          ^^
  ```

- Warning: `conf/modules/sentieon_tnscope.config:28:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { meta.num_intervals > 1 ? null : "sentieon_tnscope/${meta.id}/${it}" }
                                                                                       ^^
  ```

- Warning: `conf/modules/strelka.config:26:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { meta.num_intervals > 1 ? null : "strelka/${meta.id}/${it}" }
                                                                              ^^
  ```

- Warning: `main.nf:93:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `main.nf:135:52`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      intervals_bed_combined = params.no_intervals ? Channel.value([]) : PREPARE_INTERVALS.out.intervals_bed_combined
                                                     ^^^^^^^
  ```

- Warning: `main.nf:136:59`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      intervals_bed_gz_tbi_combined = params.no_intervals ? Channel.value([]) : PREPARE_INTERVALS.out.intervals_bed_gz_tbi_combined
                                                            ^^^^^^^
  ```

- Warning: `main.nf:142:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.value([[id: 'null'], []])
            ^^^^^^^
  ```

- Warning: `main.nf:158:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              cnvkit_reference = Channel.fromPath(params.cnvkit_reference).collect()
                                 ^^^^^^^
  ```

- Warning: `main.nf:167:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          cnvkit_reference = Channel.value([])
                             ^^^^^^^
  ```

- Warning: `main.nf:182:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ensemblvep_info = Channel.of([[id: "${params.vep_cache_version}_${params.vep_genome}"], params.vep_genome, params.vep_species, params.vep_cache_version])
                            ^^^^^^^
  ```

- Warning: `main.nf:183:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          snpeff_info = Channel.of([[id: "${params.snpeff_db}"], params.snpeff_db])
                        ^^^^^^^
  ```

- Warning: `main.nf:270:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_snpsift_db = Channel.value([[], [], [], [], []])
                      ^^^^^^^
  ```

- Warning: `main.nf:292:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          params.bcftools_columns ? Channel.fromPath(params.bcftools_columns).collect() : Channel.value([]),
                                    ^^^^^^^
  ```

- Warning: `main.nf:292:89`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          params.bcftools_columns ? Channel.fromPath(params.bcftools_columns).collect() : Channel.value([]),
                                                                                          ^^^^^^^
  ```

- Warning: `main.nf:293:40`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          params.bcftools_header_lines ? Channel.fromPath(params.bcftools_header_lines).collect() : Channel.empty(),
                                         ^^^^^^^
  ```

- Warning: `main.nf:293:99`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          params.bcftools_header_lines ? Channel.fromPath(params.bcftools_header_lines).collect() : Channel.empty(),
                                                                                                    ^^^^^^^
  ```

- Warning: `main.nf:294:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          params.cf_chrom_len ? Channel.fromPath(params.cf_chrom_len).collect() : [],
                                ^^^^^^^
  ```

- Warning: `main.nf:299:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          params.dbsnp_vqsr ? Channel.value(params.dbsnp_vqsr) : Channel.empty(),
                              ^^^^^^^
  ```

- Warning: `main.nf:299:64`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          params.dbsnp_vqsr ? Channel.value(params.dbsnp_vqsr) : Channel.empty(),
                                                                 ^^^^^^^
  ```

- Warning: `main.nf:312:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          params.known_indels_vqsr ? Channel.value(params.known_indels_vqsr) : Channel.empty(),
                                     ^^^^^^^
  ```

- Warning: `main.nf:312:78`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          params.known_indels_vqsr ? Channel.value(params.known_indels_vqsr) : Channel.empty(),
                                                                               ^^^^^^^
  ```

- Warning: `main.nf:317:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          params.known_snps_vqsr ? Channel.value(params.known_snps_vqsr) : Channel.empty(),
                                   ^^^^^^^
  ```

- Warning: `main.nf:317:74`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          params.known_snps_vqsr ? Channel.value(params.known_snps_vqsr) : Channel.empty(),
                                                                           ^^^^^^^
  ```

- Warning: `main.nf:318:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          params.mappability ? Channel.fromPath(params.mappability).collect() : Channel.value([]),
                               ^^^^^^^
  ```

- Warning: `main.nf:318:79`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          params.mappability ? Channel.fromPath(params.mappability).collect() : Channel.value([]),
                                                                                ^^^^^^^
  ```

- Warning: `main.nf:321:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          params.ngscheckmate_bed ? Channel.value(params.ngscheckmate_bed) : Channel.empty(),
                                    ^^^^^^^
  ```

- Warning: `main.nf:321:76`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          params.ngscheckmate_bed ? Channel.value(params.ngscheckmate_bed) : Channel.empty(),
                                                                             ^^^^^^^
  ```

- Warning: `main.nf:324:42`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          params.sentieon_dnascope_model ? Channel.fromPath(params.sentieon_dnascope_model).collect() : Channel.value([]),
                                           ^^^^^^^
  ```

- Warning: `main.nf:324:103`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          params.sentieon_dnascope_model ? Channel.fromPath(params.sentieon_dnascope_model).collect() : Channel.value([]),
                                                                                                        ^^^^^^^
  ```

- Warning: `main.nf:325:50`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          params.varlociraptor_scenario_germline ? Channel.fromPath(params.varlociraptor_scenario_germline).map { it -> [[id: it.baseName - '.yte'], it] }.collect() : Channel.fromPath("${projectDir}/assets/varlociraptor_germline.yte.yaml").collect(),
                                                   ^^^^^^^
  ```

- Warning: `main.nf:325:166`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          params.varlociraptor_scenario_germline ? Channel.fromPath(params.varlociraptor_scenario_germline).map { it -> [[id: it.baseName - '.yte'], it] }.collect() : Channel.fromPath("${projectDir}/assets/varlociraptor_germline.yte.yaml").collect(),
                                                                                                                                                                       ^^^^^^^
  ```

- Warning: `main.nf:326:49`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          params.varlociraptor_scenario_somatic ? Channel.fromPath(params.varlociraptor_scenario_somatic).map { it -> [[id: it.baseName - '.yte'], it] }.collect() : Channel.fromPath("${projectDir}/assets/varlociraptor_somatic.yte.yaml").collect(),
                                                  ^^^^^^^
  ```

- Warning: `main.nf:326:164`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          params.varlociraptor_scenario_somatic ? Channel.fromPath(params.varlociraptor_scenario_somatic).map { it -> [[id: it.baseName - '.yte'], it] }.collect() : Channel.fromPath("${projectDir}/assets/varlociraptor_somatic.yte.yaml").collect(),
                                                                                                                                                                     ^^^^^^^
  ```

- Warning: `main.nf:327:52`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          params.varlociraptor_scenario_tumor_only ? Channel.fromPath(params.varlociraptor_scenario_tumor_only).map { it -> [[id: it.baseName - '.yte'], it] }.collect() : Channel.fromPath("${projectDir}/assets/varlociraptor_tumor_only.yte.yaml").collect(),
                                                     ^^^^^^^
  ```

- Warning: `main.nf:327:170`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          params.varlociraptor_scenario_tumor_only ? Channel.fromPath(params.varlociraptor_scenario_tumor_only).map { it -> [[id: it.baseName - '.yte'], it] }.collect() : Channel.fromPath("${projectDir}/assets/varlociraptor_tumor_only.yte.yaml").collect(),
                                                                                                                                                                           ^^^^^^^
  ```

- Warning: `modules/local/consensus_from_sites/main.nf:27:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/bcftools/concat/main.nf:32:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input = vcfs.sort{it.toString()}.join(" ")
                            ^^
  ```

- Warning: `modules/nf-core/bcftools/isec/main.nf:35:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args   ?: ''
          ^^^^
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

- Warning: `modules/nf-core/cnvkit/batch/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def tumor_bam = tumor_exists && tumor.Extension == "bam" ? true : false
          ^^^^^^^^^
  ```

- Warning: `modules/nf-core/cnvkit/batch/main.nf:41:9`: Variable was declared but not used

  ```nextflow
      def normal_bam = normal_exists && normal.Extension == "bam" ? true : false
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/fgbio/fastqtobam/main.nf:58:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/gatk4/baserecalibrator/main.nf:29:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def sites_command = known_sites.collect{"--known-sites $it"}.join(' ')
                                                             ^^
  ```

- Warning: `modules/nf-core/gatk4/estimatelibrarycomplexity/main.nf:26:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = input.collect(){"--INPUT $it"}.join(" ")
                                                ^^
  ```

- Warning: `modules/nf-core/gatk4/filtermutectcalls/main.nf:29:113`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def orientationbias_command = orientationbias ? orientationbias.collect{"--orientation-bias-artifact-priors $it"}.join(' ') : ''
                                                                                                                  ^^
  ```

- Warning: `modules/nf-core/gatk4/filtermutectcalls/main.nf:30:96`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def segmentation_command    = segmentation    ? segmentation.collect{"--tumor-segmentation $it"}.join(' ')                  : ''
                                                                                                 ^^
  ```

- Warning: `modules/nf-core/gatk4/filtermutectcalls/main.nf:32:90`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def table_command           = table           ? table.collect{"--contamination-table $it"}.join(' ')                        : ''
                                                                                           ^^
  ```

- Warning: `modules/nf-core/gatk4/filtervarianttranches/main.nf:30:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def resource_list = resources.collect{"--resource $it"}.join(' ')
                                                        ^^
  ```

- Warning: `modules/nf-core/gatk4/gatherbqsrreports/main.nf:23:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = table.collect{"--input $it"}.join(' ')
                                              ^^
  ```

- Warning: `modules/nf-core/gatk4/gatherpileupsummaries/main.nf:25:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = pileup.collect{ "--I $it" }.join(' ')
                                            ^^
  ```

- Warning: `modules/nf-core/gatk4/genomicsdbimport/main.nf:30:90`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      input_command = input_map ? "--sample-name-map ${vcf[0]}" : vcf.collect(){"--variant $it"}.join(' ')
                                                                                           ^^
  ```

- Warning: `modules/nf-core/gatk4/learnreadorientationmodel/main.nf:23:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = f1r2.collect{"--input $it"}.join(' ')
                                             ^^
  ```

- Warning: `modules/nf-core/gatk4/markduplicates/main.nf:33:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = bam.collect { "--INPUT ${it}" }.join(' ')
                                                ^^
  ```

- Warning: `modules/nf-core/gatk4/mergemutectstats/main.nf:23:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = stats.collect{ "--stats ${it}"}.join(' ')
                                                 ^^
  ```

- Warning: `modules/nf-core/gatk4/mergevcfs/main.nf:25:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = vcf.collect{ "--INPUT $it"}.join(' ')
                                             ^^
  ```

- Warning: `modules/nf-core/gatk4/mutect2/main.nf:33:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def inputs = input.collect{ "--input $it"}.join(" ")
                                           ^^
  ```

- Warning: `modules/nf-core/gatk4spark/baserecalibrator/main.nf:29:64`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def sites_command = known_sites.collect { "--known-sites ${it}" }.join(' ')
                                                                 ^^
  ```

- Warning: `modules/nf-core/gatk4spark/markduplicates/main.nf:28:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = bam.collect { "--input ${it}" }.join(' ')
                                                ^^
  ```

- Warning: `modules/nf-core/gawk/main.nf:26:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      suffix    = task.ext.suffix ?: "${input.collect{ it.getExtension()}.get(0)}" // use the first extension of the input files
                                                       ^^
  ```

- Warning: `modules/nf-core/gawk/main.nf:29:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      lst_gz     = input.findResults{ it.getExtension().endsWith("gz") ? it.toString() : null }
                                      ^^
  ```

- Warning: `modules/nf-core/gawk/main.nf:29:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      lst_gz     = input.findResults{ it.getExtension().endsWith("gz") ? it.toString() : null }
                                                                         ^^
  ```

- Warning: `modules/nf-core/gawk/main.nf:31:34`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      input_cmd  = input.collect { it.toString() - ~/\.gz$/ }.join(" ")
                                   ^^
  ```

- Warning: `modules/nf-core/gawk/main.nf:34:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      cleanup    = lst_gz ? "rm ${lst_gz.collect{ it - ~/\.gz$/ }.join(" ")}" : ""
                                                  ^^
  ```

- Warning: `modules/nf-core/gawk/main.nf:37:16`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          assert it.name != "${prefix}.${suffix}" : "Input and output names are the same, set prefix in module configuration to disambiguate!"
                 ^^
  ```

- Warning: `modules/nf-core/goleft/indexcov/main.nf:31:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_files = bams.findAll{it.name.endsWith(".bam")} + indexes.findAll{it.name.endsWith(".crai")}
                                     ^^
  ```

- Warning: `modules/nf-core/goleft/indexcov/main.nf:31:80`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_files = bams.findAll{it.name.endsWith(".bam")} + indexes.findAll{it.name.endsWith(".crai")}
                                                                                 ^^
  ```

- Warning: `modules/nf-core/goleft/indexcov/main.nf:32:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def extranormalize = input_files.any{it.name.endsWith(".crai")} ? " --extranormalize " : ""
                                           ^^
  ```

- Warning: `modules/nf-core/goleft/indexcov/main.nf:52:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/gunzip/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/lofreq/callparallel/main.nf:29:9`: Variable was declared but not used

  ```nextflow
      def alignment_bam = bam.Extension == "bam" ? true : false
          ^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/manta/germline/main.nf:33:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_files = input.collect{"--bam ${it}"}.join(' ')
                                               ^^
  ```

- Warning: `modules/nf-core/ngscheckmate/ncm/main.nf:28:29`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def unzip = files.any { it.toString().endsWith(".vcf.gz") }
                              ^^
  ```

- Warning: `modules/nf-core/ngscheckmate/ncm/main.nf:51:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/sentieon/dedup/main.nf:36:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = bam.collect { "-i ${it}" }.join(' ')
                                           ^^
  ```

- Warning: `modules/nf-core/sentieon/haplotyper/main.nf:37:68`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = input instanceof List ? input.collect { "-i ${it}" }.join(' ') : "-i ${input}"
                                                                     ^^
  ```

- Warning: `modules/nf-core/sentieon/tnscope/main.nf:38:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def inputs = input.collect { "-i ${it}" }.join(" ")
                                         ^^
  ```

- Warning: `modules/nf-core/svdb/merge/main.nf:38:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def pairs = vcfs.indices.collect { [vcfs[it], input_priority[it]] }
                                                      ^^
  ```

- Warning: `modules/nf-core/svdb/merge/main.nf:38:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def pairs = vcfs.indices.collect { [vcfs[it], input_priority[it]] }
                                                                          ^^
  ```

- Warning: `modules/nf-core/svdb/merge/main.nf:40:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              vcfs = pairs.collect { it[0] }
                                     ^^
  ```

- Warning: `modules/nf-core/svdb/merge/main.nf:41:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              priority = pairs.collect { it[1] }
                                         ^^
  ```

- Warning: `modules/nf-core/svdb/merge/main.nf:55:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          input = (vcfs.collect().size() > 1 && sort_inputs) ? vcfs.sort { it.name } : vcfs
                                                                           ^^
  ```

- Warning: `modules/nf-core/unzip/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/vcftools/main.nf:97:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      args_list.removeIf { it.contains('--bed') }
                           ^^
  ```

- Warning: `modules/nf-core/vcftools/main.nf:98:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      args_list.removeIf { it.contains('--exclude-bed') }
                           ^^
  ```

- Warning: `modules/nf-core/vcftools/main.nf:99:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      args_list.removeIf { it.contains('--hapcount') }
                           ^^
  ```

- Warning: `modules/nf-core/vcftools/main.nf:100:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      args_list.removeIf { it.contains('--positions') }
                           ^^
  ```

- Warning: `modules/nf-core/vcftools/main.nf:101:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      args_list.removeIf { it.contains('--exclude-positions') }
                           ^^
  ```

- Warning: `modules/nf-core/vcftools/main.nf:106:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      args_list.removeIf { it.contains('--diff') }
                           ^^
  ```

- Warning: `modules/nf-core/vcftools/main.nf:107:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      args_list.removeIf { it.contains('--gzdiff') }
                           ^^
  ```

- Warning: `modules/nf-core/vcftools/main.nf:108:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      args_list.removeIf { it.contains('--diff-bcf') }
                           ^^
  ```

- Warning: `subworkflows/local/annotation_cache_initialisation/main.nf:37:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          snpeff_cache = Channel.fromPath(file("${snpeff_cache}/${snpeff_annotation_cache_key}"), checkIfExists: true)
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/annotation_cache_initialisation/main.nf:58:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ensemblvep_cache = Channel.fromPath(file("${vep_cache}/${vep_annotation_cache_key}"), checkIfExists: true).collect()
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_baserecalibrator/main.nf:21:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_baserecalibrator/main.nf:41:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          single:   it[0].num_intervals <= 1
                    ^^
  ```

- Warning: `subworkflows/local/bam_baserecalibrator/main.nf:42:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          multiple: it[0].num_intervals > 1
                    ^^
  ```

- Warning: `subworkflows/local/bam_baserecalibrator/main.nf:49:5`: Variable was declared but not used

  ```nextflow
      table_bqsr = GATK4_GATHERBQSRREPORTS.out.table.mix(table_to_merge.single.map{ meta, table -> [ meta, table[0] ] })
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_baserecalibrator_spark/main.nf:21:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_baserecalibrator_spark/main.nf:29:60`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      GATK4SPARK_BASERECALIBRATOR(cram_intervals, fasta.map{ meta, it -> [ it ] }, fasta_fai.map{ meta, it -> [ it ] }, dict.map{ meta, it -> [ it ] }, known_sites, known_sites_tbi)
                                                             ^^^^
  ```

- Warning: `subworkflows/local/bam_baserecalibrator_spark/main.nf:29:97`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      GATK4SPARK_BASERECALIBRATOR(cram_intervals, fasta.map{ meta, it -> [ it ] }, fasta_fai.map{ meta, it -> [ it ] }, dict.map{ meta, it -> [ it ] }, known_sites, known_sites_tbi)
                                                                                                  ^^^^
  ```

- Warning: `subworkflows/local/bam_baserecalibrator_spark/main.nf:29:129`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      GATK4SPARK_BASERECALIBRATOR(cram_intervals, fasta.map{ meta, it -> [ it ] }, fasta_fai.map{ meta, it -> [ it ] }, dict.map{ meta, it -> [ it ] }, known_sites, known_sites_tbi)
                                                                                                                                  ^^^^
  ```

- Warning: `subworkflows/local/bam_baserecalibrator_spark/main.nf:34:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          single:   it[0].num_intervals <= 1
                    ^^
  ```

- Warning: `subworkflows/local/bam_baserecalibrator_spark/main.nf:35:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          multiple: it[0].num_intervals > 1
                    ^^
  ```

- Warning: `subworkflows/local/bam_baserecalibrator_spark/main.nf:42:5`: Variable was declared but not used

  ```nextflow
      table_bqsr = GATK4_GATHERBQSRREPORTS.out.table.mix(table_to_merge.single.map{ meta, table -> [ meta, table[0] ] })
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_convert_samtools/main.nf:22:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_convert_samtools/main.nf:60:5`: Variable was declared but not used

  ```nextflow
      reads = CAT_FASTQ.out.reads
      ^^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_gatk/main.nf:34:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_gatk/main.nf:74:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          fasta.map{ meta, fasta_ -> [ fasta_ ] },
                     ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_gatk/main.nf:75:18`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          fai.map{ meta, fai_ -> [ fai_ ] },
                   ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_gatk/main.nf:76:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          dict.map{ meta, dict_ -> [ dict_ ] })
                    ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_gatk/main.nf:83:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          fasta.map{ meta, fasta_ -> [ fasta_ ] },
                     ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_gatk/main.nf:84:18`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          fai.map{ meta, fai_ -> [ fai_ ] },
                   ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_gatk/main.nf:85:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          dict.map{ meta, dict_ -> [ dict_ ] })
                    ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_gatk/main.nf:100:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          fasta.map{ meta, fasta_ -> [ fasta_ ] },
                     ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_gatk/main.nf:101:18`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          fai.map{ meta, fai_ -> [ fai_ ] },
                   ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_gatk/main.nf:102:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          dict.map{ meta, dict_ -> [ dict_ ] })
                    ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_gatk/main.nf:114:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          fasta.map{ meta, fasta_ -> [ fasta_ ] },
                     ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_gatk/main.nf:115:18`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          fai.map{ meta, fai_ -> [ fai_ ] },
                   ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_gatk/main.nf:116:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          dict.map{ meta, dict_ -> [ dict_ ] })
                    ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_gatk/main.nf:123:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      merge_vcf_for_join = MERGE_GENOTYPEGVCFS.out.vcf.map{meta, vcf -> [[id: 'joint_variant_calling'] , vcf]}
                                                           ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_gatk/main.nf:124:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      merge_tbi_for_join = MERGE_GENOTYPEGVCFS.out.tbi.map{meta, tbi -> [[id: 'joint_variant_calling'] , tbi]}
                                                           ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_gatk/main.nf:127:78`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      vqsr_vcf_for_join = GATK4_APPLYVQSR_INDEL.out.vcf.ifEmpty([[:], []]).map{meta, vcf -> [[id: 'joint_variant_calling'] , vcf]}
                                                                               ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_gatk/main.nf:128:78`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      vqsr_tbi_for_join = GATK4_APPLYVQSR_INDEL.out.tbi.ifEmpty([[:], []]).map{meta, tbi -> [[id: 'joint_variant_calling'] , tbi]}
                                                                               ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_gatk/main.nf:134:5`: Variable was declared but not used

  ```nextflow
      genotype_vcf = merge_vcf_for_join.join(vqsr_vcf_for_join, remainder: true).map{
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_gatk/main.nf:135:9`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          meta, joint_vcf, recal_vcf ->
          ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_gatk/main.nf:142:5`: Variable was declared but not used

  ```nextflow
      genotype_index = merge_tbi_for_join.join(vqsr_tbi_for_join, remainder: true).map{
      ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_gatk/main.nf:143:9`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          meta, joint_tbi, recal_tbi ->
          ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_sentieon/main.nf:33:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_sentieon/main.nf:54:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      merged_vcf = MERGE_GENOTYPEGVCFS.out.vcf.map{meta, vcf -> [[id: 'joint_variant_calling'] , vcf]}
                                                   ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_sentieon/main.nf:55:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      merged_tbi = MERGE_GENOTYPEGVCFS.out.tbi.map{meta, tbi -> [[id: 'joint_variant_calling'] , tbi]}
                                                   ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_sentieon/main.nf:76:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              fasta.map{meta, it -> [ it ]},
                        ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_sentieon/main.nf:77:21`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              fai.map{meta, it -> [ it ]})
                      ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_sentieon/main.nf:84:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              fasta.map{meta, it -> [ it ]},
                        ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_sentieon/main.nf:85:21`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              fai.map{meta, it -> [ it ]})
                      ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_sentieon/main.nf:115:87`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          vqsr_vcf_for_join = SENTIEON_APPLYVARCAL_INDEL.out.vcf.ifEmpty([[:], []]).map{meta, vcf -> [[id: 'joint_variant_calling'] , vcf]}
                                                                                        ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_sentieon/main.nf:116:87`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          vqsr_tbi_for_join = SENTIEON_APPLYVARCAL_INDEL.out.tbi.ifEmpty([[:], []]).map{meta, tbi -> [[id: 'joint_variant_calling'] , tbi]}
                                                                                        ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_sentieon/main.nf:123:13`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, joint_vcf, recal_vcf ->
              ^^^^
  ```

- Warning: `subworkflows/local/bam_joint_calling_germline_sentieon/main.nf:131:13`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, joint_tbi, recal_tbi ->
              ^^^^
  ```

- Warning: `subworkflows/local/bam_markduplicates/main.nf:18:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_markduplicates/main.nf:19:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      reports  = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_markduplicates/main.nf:22:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      GATK4_MARKDUPLICATES(bam, fasta.map{ meta, fasta_ -> [ fasta_ ] }, fasta_fai.map{ meta, fasta_fai_ -> [ fasta_fai_ ] })
                                           ^^^^
  ```

- Warning: `subworkflows/local/bam_markduplicates/main.nf:22:87`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      GATK4_MARKDUPLICATES(bam, fasta.map{ meta, fasta_ -> [ fasta_ ] }, fasta_fai.map{ meta, fasta_fai_ -> [ fasta_fai_ ] })
                                                                                        ^^^^
  ```

- Warning: `subworkflows/local/bam_markduplicates_spark/main.nf:21:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_markduplicates_spark/main.nf:22:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      reports = Channel.empty()
                ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_markduplicates_spark/main.nf:25:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      GATK4SPARK_MARKDUPLICATES(bam, fasta.map{ meta, fasta_ -> [ fasta_ ] }, fasta_fai.map{ meta, fasta_fai_ -> [ fasta_fai_ ] }, dict.map{ meta, dict_ -> [ dict_ ] })
                                                ^^^^
  ```

- Warning: `subworkflows/local/bam_markduplicates_spark/main.nf:25:92`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      GATK4SPARK_MARKDUPLICATES(bam, fasta.map{ meta, fasta_ -> [ fasta_ ] }, fasta_fai.map{ meta, fasta_fai_ -> [ fasta_fai_ ] }, dict.map{ meta, dict_ -> [ dict_ ] })
                                                                                             ^^^^
  ```

- Warning: `subworkflows/local/bam_markduplicates_spark/main.nf:25:140`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      GATK4SPARK_MARKDUPLICATES(bam, fasta.map{ meta, fasta_ -> [ fasta_ ] }, fasta_fai.map{ meta, fasta_fai_ -> [ fasta_fai_ ] }, dict.map{ meta, dict_ -> [ dict_ ] })
                                                                                                                                             ^^^^
  ```

- Warning: `subworkflows/local/bam_markduplicates_spark/main.nf:37:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      GATK4_ESTIMATELIBRARYCOMPLEXITY(bam, fasta.map{ meta, fasta_ -> [ fasta_ ] }, fasta_fai.map{ meta, fasta_fai_ -> [ fasta_fai_ ] }, dict.map{ meta, dict_ -> [ dict_ ] })
                                                      ^^^^
  ```

- Warning: `subworkflows/local/bam_markduplicates_spark/main.nf:37:98`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      GATK4_ESTIMATELIBRARYCOMPLEXITY(bam, fasta.map{ meta, fasta_ -> [ fasta_ ] }, fasta_fai.map{ meta, fasta_fai_ -> [ fasta_fai_ ] }, dict.map{ meta, dict_ -> [ dict_ ] })
                                                                                                   ^^^^
  ```

- Warning: `subworkflows/local/bam_markduplicates_spark/main.nf:37:146`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      GATK4_ESTIMATELIBRARYCOMPLEXITY(bam, fasta.map{ meta, fasta_ -> [ fasta_ ] }, fasta_fai.map{ meta, fasta_fai_ -> [ fasta_fai_ ] }, dict.map{ meta, dict_ -> [ dict_ ] })
                                                                                                                                                   ^^^^
  ```

- Warning: `subworkflows/local/bam_merge_index_samtools/main.nf:15:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_merge_index_samtools/main.nf:35:5`: Variable was declared but not used

  ```nextflow
      bam_bai = bam_all.join(INDEX_MERGE_BAM.out.bai, failOnDuplicate: true, failOnMismatch: true)
      ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_sentieon_dedup/main.nf:16:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_sentieon_dedup/main.nf:17:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      reports  = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_cnvkit/main.nf:21:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_deepvariant/main.nf:21:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_deepvariant/main.nf:33:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_deepvariant/main.nf:34:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_deepvariant/main.nf:40:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_deepvariant/main.nf:41:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_deepvariant/main.nf:54:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_deepvariant/main.nf:55:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_deepvariant/main.nf:59:5`: Variable was declared but not used

  ```nextflow
      gvcf = Channel.empty().mix(MERGE_DEEPVARIANT_GVCF.out.vcf, gvcf_out.no_intervals)
      ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_deepvariant/main.nf:59:12`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      gvcf = Channel.empty().mix(MERGE_DEEPVARIANT_GVCF.out.vcf, gvcf_out.no_intervals)
             ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_deepvariant/main.nf:64:5`: Variable was declared but not used

  ```nextflow
      vcf = Channel.empty().mix(MERGE_DEEPVARIANT_VCF.out.vcf, vcf_out.no_intervals)
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_deepvariant/main.nf:64:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf = Channel.empty().mix(MERGE_DEEPVARIANT_VCF.out.vcf, vcf_out.no_intervals)
            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_deepvariant/main.nf:68:5`: Variable was declared but not used

  ```nextflow
      tbi = Channel.empty().mix(MERGE_DEEPVARIANT_VCF.out.tbi, tbi_out.no_intervals)
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_deepvariant/main.nf:68:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi = Channel.empty().mix(MERGE_DEEPVARIANT_VCF.out.tbi, tbi_out.no_intervals)
            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_freebayes/main.nf:23:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_freebayes/main.nf:37:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_freebayes/main.nf:38:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:26:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      bam                               // channel: [mandatory] meta, bam
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:55:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:58:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      gvcf_sentieon_dnascope   = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:59:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      gvcf_sentieon_haplotyper = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:61:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      out_indexcov             = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:62:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_deepvariant          = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:63:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_freebayes            = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:64:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_haplotypecaller      = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:65:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_manta                = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:66:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_mpileup              = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:67:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_sentieon_dnascope    = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:68:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_sentieon_haplotyper  = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:69:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_strelka              = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:70:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_tiddit               = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:71:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi_deepvariant          = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:72:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi_freebayes            = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:73:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi_haplotypecaller      = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:74:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi_manta                = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:75:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi_mpileup              = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:76:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi_sentieon_dnascope    = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:77:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi_sentieon_haplotyper  = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:78:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi_strelka              = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:79:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi_tiddit               = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:98:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              cram.map{ meta, cram_, crai -> [ meta, [], cram_ ] },
                                     ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:181:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      fasta.map{ meta, fasta_ -> [ fasta_ ] },
                                 ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:182:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      fasta_fai.map{ meta, fasta_fai_ -> [ fasta_fai_ ] },
                                     ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:183:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      dict.map{ meta, dict_ -> [ dict_ ] },
                                ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:243:9`: Variable was declared but not used

  ```nextflow
          gvcf_tbi_sentieon_dnascope = BAM_VARIANT_CALLING_SENTIEON_DNASCOPE.out.gvcf_tbi
          ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:303:9`: Variable was declared but not used

  ```nextflow
          gvcf_tbi_sentieon_haplotyper = BAM_VARIANT_CALLING_SENTIEON_HAPLOTYPER.out.gvcf_tbi
          ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:332:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      fasta.map{ meta, it -> [ it ] },
                                 ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:333:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      fasta_fai.map{ meta, it -> [ it ] },
                                     ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:334:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      dict.map{ meta, dict_ -> [ dict_ ] },
                                ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:354:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              fasta.map{ meta, fasta_ -> [ fasta_ ] },
                         ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:355:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              fasta_fai.map{ meta, fasta_fai_ -> [ fasta_fai_ ] },
                             ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:378:5`: Variable was declared but not used

  ```nextflow
      vcf_all = Channel.empty().mix(
      ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:378:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_all = Channel.empty().mix(
                ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:390:5`: Variable was declared but not used

  ```nextflow
      tbi_all = Channel.empty().mix(
      ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:390:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi_all = Channel.empty().mix(
                ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_manta/main.nf:18:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_manta/main.nf:30:5`: Variable was declared but not used

  ```nextflow
      small_indels_vcf     = MANTA_GERMLINE.out.candidate_small_indels_vcf
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_manta/main.nf:31:5`: Variable was declared but not used

  ```nextflow
      sv_vcf               = MANTA_GERMLINE.out.candidate_sv_vcf
      ^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_manta/main.nf:37:5`: Variable was declared but not used

  ```nextflow
      vcf = diploid_sv_vcf.map{ meta, vcf -> [ meta + [ variantcaller:'manta' ], vcf ] }
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_manta/main.nf:38:5`: Variable was declared but not used

  ```nextflow
      tbi = diploid_sv_vcf_tbi.map{ meta, tbi -> [ meta + [ variantcaller:'manta' ], tbi ] }
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_haplotypecaller/main.nf:22:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_haplotypecaller/main.nf:24:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf           = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_haplotypecaller/main.nf:25:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      realigned_bam = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_haplotypecaller/main.nf:42:5`: Variable was declared but not used

  ```nextflow
      gvcf_tbi_intervals = GATK4_HAPLOTYPECALLER.out.vcf
      ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_haplotypecaller/main.nf:45:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta, gvcf, tbi, cram_, crai, intervals_, dragstr_model -> [ meta, gvcf, tbi, intervals_ ] }
                                 ^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_haplotypecaller/main.nf:45:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta, gvcf, tbi, cram_, crai, intervals_, dragstr_model -> [ meta, gvcf, tbi, intervals_ ] }
                                        ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_haplotypecaller/main.nf:45:57`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta, gvcf, tbi, cram_, crai, intervals_, dragstr_model -> [ meta, gvcf, tbi, intervals_ ] }
                                                          ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_haplotypecaller/main.nf:53:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              intervals:    it[0].num_intervals > 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_haplotypecaller/main.nf:54:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_intervals: it[0].num_intervals <= 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_haplotypecaller/main.nf:62:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              intervals:    it[0].num_intervals > 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_haplotypecaller/main.nf:63:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_intervals: it[0].num_intervals <= 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_haplotypecaller/main.nf:71:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              intervals:    it[0].num_intervals > 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_haplotypecaller/main.nf:72:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_intervals: it[0].num_intervals <= 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_haplotypecaller/main.nf:78:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      haplotypecaller_vcf = Channel.empty().mix(
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_haplotypecaller/main.nf:82:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      haplotypecaller_tbi = Channel.empty().mix(
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_haplotypecaller/main.nf:99:5`: Variable was declared but not used

  ```nextflow
      tbi = haplotypecaller_tbi.map{ meta, tbi -> [ meta - meta.subMap('num_intervals'), tbi ] }
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_indexcov/main.nf:18:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_indexcov/main.nf:30:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      indexcov_input_ch = reindex_ch.output.map{[[id:"indexcov"], it[1], it[2]]}.groupTuple()
                                                                  ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_indexcov/main.nf:30:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      indexcov_input_ch = reindex_ch.output.map{[[id:"indexcov"], it[1], it[2]]}.groupTuple()
                                                                         ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_mpileup/main.nf:20:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_mpileup/main.nf:36:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_mpileup/main.nf:37:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_mpileup/main.nf:42:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_mpileup/main.nf:43:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_mpileup/main.nf:48:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_mpileup/main.nf:49:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_mpileup/main.nf:61:5`: Variable was declared but not used

  ```nextflow
      mpileup = CAT_MPILEUP.out.file_out
      ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_mpileup/main.nf:64:5`: Variable was declared but not used

  ```nextflow
      vcf = MERGE_BCFTOOLS_MPILEUP.out.vcf
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_mpileup/main.nf:67:5`: Variable was declared but not used

  ```nextflow
      tbi = MERGE_BCFTOOLS_MPILEUP.out.tbi
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:19:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      dbsnp_vqsr                        // channel: [optional]
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:27:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:29:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      gvcf               = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:30:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf                = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:31:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      genotype_intervals = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:60:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          emit_mode_items.any{ it.equals('gvcf') })
                               ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:66:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map{ meta, gvcf_, tbi, cram_, crai, intervals_ -> [ meta, gvcf_, tbi, intervals_ ] }
                                      ^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:66:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map{ meta, gvcf_, tbi, cram_, crai, intervals_ -> [ meta, gvcf_, tbi, intervals_ ] }
                                             ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:74:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              intervals:    it[0].num_intervals > 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:75:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_intervals: it[0].num_intervals <= 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:82:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              intervals:    it[0].num_intervals > 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:83:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_intervals: it[0].num_intervals <= 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:90:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              intervals:    it[0].num_intervals > 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:91:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_intervals: it[0].num_intervals <= 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:98:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              intervals:    it[0].num_intervals > 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:99:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_intervals: it[0].num_intervals <= 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:114:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      dnascope_vcf = Channel.empty().mix(
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:118:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      haplotyper_tbi = Channel.empty().mix(
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:124:5`: Variable was declared but not used

  ```nextflow
      vcf_tbi = haplotyper_tbi.map{ meta, tbi -> [ meta - meta.subMap('num_intervals'), tbi ] }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:137:12`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      gvcf = Channel.empty().mix(
             ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:141:5`: Variable was declared but not used

  ```nextflow
      gvcf_tbi = Channel.empty().mix(
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:141:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      gvcf_tbi = Channel.empty().mix(
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:19:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      dbsnp_vqsr                     // channel: [optional]
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:25:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:27:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      gvcf               = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:28:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf                = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:29:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      genotype_intervals = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:56:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          emit_mode_items.any{ it.equals('gvcf') })
                               ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:62:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map{ meta, gvcf_, tbi, cram_, crai, intervals_ -> [ meta, gvcf_, tbi, intervals_ ] }
                                      ^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:62:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map{ meta, gvcf_, tbi, cram_, crai, intervals_ -> [ meta, gvcf_, tbi, intervals_ ] }
                                             ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:70:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              intervals:    it[0].num_intervals > 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:71:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_intervals: it[0].num_intervals <= 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:78:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              intervals:    it[0].num_intervals > 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:79:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_intervals: it[0].num_intervals <= 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:86:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              intervals:    it[0].num_intervals > 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:87:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_intervals: it[0].num_intervals <= 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:94:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              intervals:    it[0].num_intervals > 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:95:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_intervals: it[0].num_intervals <= 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:110:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      haplotyper_vcf = Channel.empty().mix(
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:114:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      haplotyper_tbi = Channel.empty().mix(
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:120:5`: Variable was declared but not used

  ```nextflow
      vcf_tbi = haplotyper_tbi.map{ meta, tbi -> [ meta - meta.subMap('num_intervals'), tbi ] }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:133:12`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      gvcf = Channel.empty().mix(
             ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:137:5`: Variable was declared but not used

  ```nextflow
      gvcf_tbi = Channel.empty().mix(
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:137:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      gvcf_tbi = Channel.empty().mix(
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_single_strelka/main.nf:20:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_single_strelka/main.nf:32:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_single_strelka/main.nf:33:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_single_strelka/main.nf:39:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_single_strelka/main.nf:40:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_single_strelka/main.nf:46:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_single_strelka/main.nf:47:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_single_strelka/main.nf:59:5`: Variable was declared but not used

  ```nextflow
      vcf = Channel.empty().mix(MERGE_STRELKA.out.vcf, vcf_out.no_intervals)
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_single_strelka/main.nf:59:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf = Channel.empty().mix(MERGE_STRELKA.out.vcf, vcf_out.no_intervals)
            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_single_strelka/main.nf:63:5`: Variable was declared but not used

  ```nextflow
      tbi = Channel.empty().mix(MERGE_STRELKA.out.tbi, tbi_out.no_intervals)
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_single_strelka/main.nf:63:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi = Channel.empty().mix(MERGE_STRELKA.out.tbi, tbi_out.no_intervals)
            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_single_tiddit/main.nf:23:5`: Variable was declared but not used

  ```nextflow
      ploidy = TIDDIT_SV.out.ploidy
      ^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_single_tiddit/main.nf:24:5`: Variable was declared but not used

  ```nextflow
      vcf = TABIX_BGZIP_TIDDIT_SV.out.gz_index.map { meta, gz, tbi -> [meta + [variantcaller: 'tiddit'], gz] }
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_single_tiddit/main.nf:24:62`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      vcf = TABIX_BGZIP_TIDDIT_SV.out.gz_index.map { meta, gz, tbi -> [meta + [variantcaller: 'tiddit'], gz] }
                                                               ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_single_tiddit/main.nf:25:5`: Variable was declared but not used

  ```nextflow
      tbi = TABIX_BGZIP_TIDDIT_SV.out.gz_index.map { meta, gz, tbi -> [meta + [variantcaller: 'tiddit'], tbi] }
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_single_tiddit/main.nf:25:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      tbi = TABIX_BGZIP_TIDDIT_SV.out.gz_index.map { meta, gz, tbi -> [meta + [variantcaller: 'tiddit'], tbi] }
                                                           ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_all/main.nf:289:5`: Variable was declared but not used

  ```nextflow
      vcf_all = channel.empty()
      ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_all/main.nf:300:5`: Variable was declared but not used

  ```nextflow
      tbi_all = channel.empty()
      ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_ascat/main.nf:22:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_controlfreec/main.nf:26:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_controlfreec/main.nf:34:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def tumor_file = cnv instanceof List ? cnv.find { it.toString().endsWith("gz_CNVs") } : cnv //only find if its a list, else it returns only the filename without the path
                                                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_controlfreec/main.nf:43:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def tumor_file = ratio instanceof List ? ratio.find { it.toString().endsWith("gz_ratio.txt") } : ratio //same here as cnv
                                                                ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_manta/main.nf:17:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_manta/main.nf:29:5`: Variable was declared but not used

  ```nextflow
      candidate_small_indels_vcf = MANTA_SOMATIC.out.candidate_small_indels_vcf
      ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_manta/main.nf:30:5`: Variable was declared but not used

  ```nextflow
      candidate_small_indels_vcf_tbi = MANTA_SOMATIC.out.candidate_small_indels_vcf_tbi
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_manta/main.nf:31:5`: Variable was declared but not used

  ```nextflow
      candidate_sv_vcf = MANTA_SOMATIC.out.candidate_sv_vcf
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_manta/main.nf:39:5`: Variable was declared but not used

  ```nextflow
      vcf = Channel.empty().mix(diploid_sv_vcf, somatic_sv_vcf).map{ meta, vcf -> [ meta + [ variantcaller:'manta' ], vcf ] }
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_manta/main.nf:39:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf = Channel.empty().mix(diploid_sv_vcf, somatic_sv_vcf).map{ meta, vcf -> [ meta + [ variantcaller:'manta' ], vcf ] }
            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_manta/main.nf:40:5`: Variable was declared but not used

  ```nextflow
      tbi = Channel.empty().mix(diploid_sv_vcf_tbi, somatic_sv_vcf_tbi).map{ meta, tbi -> [ meta + [ variantcaller:'manta' ], tbi ] }
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_manta/main.nf:40:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi = Channel.empty().mix(diploid_sv_vcf_tbi, somatic_sv_vcf_tbi).map{ meta, tbi -> [ meta + [ variantcaller:'manta' ], tbi ] }
            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_muse/main.nf:27:5`: Variable was declared but not used

  ```nextflow
      vcf = MUSE_SUMP.out.vcf.map { meta, vcf -> [meta + [variantcaller: 'muse'], vcf] }
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_muse/main.nf:28:5`: Variable was declared but not used

  ```nextflow
      tbi = MUSE_SUMP.out.tbi.map { meta, tbi -> [meta + [variantcaller: 'muse'], tbi] }
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:31:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:35:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      germline_resource_pileup = germline_resource.filter { it != [] }
                                                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:36:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      germline_resource_pileup_tbi = germline_resource_tbi.filter { it != [] }
                                                                    ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:72:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:73:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:78:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:79:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:84:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:85:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:90:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:91:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:103:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf = Channel.empty()
            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:108:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi = Channel.empty()
            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:113:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      stats = Channel.empty()
              ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:118:12`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      f1r2 = Channel.empty()
             ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:145:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:146:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:151:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:152:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:165:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      pileup_table_tumor = Channel.empty().mix(GATHERPILEUPSUMMARIES_TUMOR.out.table, pileup_table_tumor_branch.no_intervals).map { meta, table -> [meta - meta.subMap('normal_id', 'tumor_id', 'num_intervals') + [id: meta.patient], meta.id, table] }
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:166:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      pileup_table_normal = Channel.empty().mix(GATHERPILEUPSUMMARIES_NORMAL.out.table, pileup_table_normal_branch.no_intervals).map { meta, table -> [meta - meta.subMap('normal_id', 'tumor_id', 'num_intervals') + [id: meta.patient], meta.id, table] }
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:186:38`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      calculatecontamination_out_seg = Channel.empty()
                                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:187:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      calculatecontamination_out_cont = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:223:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .unique { it[0] }
                    ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:228:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .unique { it[0] }
                    ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:20:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:32:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:33:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:39:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:40:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:53:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:54:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:60:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:61:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:65:5`: Variable was declared but not used

  ```nextflow
      vcf = Channel.empty().mix(MERGE_STRELKA_INDELS.out.vcf, MERGE_STRELKA_SNVS.out.vcf, vcf_indels.no_intervals, vcf_snvs.no_intervals)
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:65:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf = Channel.empty().mix(MERGE_STRELKA_INDELS.out.vcf, MERGE_STRELKA_SNVS.out.vcf, vcf_indels.no_intervals, vcf_snvs.no_intervals)
            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:69:5`: Variable was declared but not used

  ```nextflow
      tbi = Channel.empty().mix(MERGE_STRELKA_INDELS.out.tbi, MERGE_STRELKA_SNVS.out.tbi, tbi_indels.no_intervals, tbi_snvs.no_intervals)
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:69:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi = Channel.empty().mix(MERGE_STRELKA_INDELS.out.tbi, MERGE_STRELKA_SNVS.out.tbi, tbi_indels.no_intervals, tbi_snvs.no_intervals)
            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_tiddit/main.nf:20:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_tiddit/main.nf:27:5`: Variable was declared but not used

  ```nextflow
      vcf = SVDB_MERGE.out.vcf.map{ meta, vcf -> [ meta + [ variantcaller:'tiddit' ], vcf ] }
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_tiddit/main.nf:28:5`: Variable was declared but not used

  ```nextflow
      tbi = SVDB_MERGE.out.tbi.map{ meta, tbi -> [ meta + [ variantcaller:'tiddit' ], tbi ] }
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_tnscope/main.nf:22:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_tnscope/main.nf:45:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_tnscope/main.nf:46:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_tnscope/main.nf:51:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_tnscope/main.nf:52:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_tnscope/main.nf:63:5`: Variable was declared but not used

  ```nextflow
      vcf   = Channel.empty()
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_tnscope/main.nf:63:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf   = Channel.empty()
              ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_tnscope/main.nf:67:5`: Variable was declared but not used

  ```nextflow
      index = Channel.empty()
      ^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_tnscope/main.nf:67:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      index = Channel.empty()
              ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_all/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      intervals_bed_gz_tbi          // channel: [mandatory] [ interval.bed.gz, interval.bed.gz.tbi, num_intervals ] or [ [], [], 0 ] if no intervals
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_all/main.nf:48:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_all/main.nf:51:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      out_msisensor2 = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_all/main.nf:52:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_freebayes  = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_all/main.nf:53:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_lofreq     = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_all/main.nf:54:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_manta      = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_all/main.nf:55:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_mpileup    = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_all/main.nf:56:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_mutect2    = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_all/main.nf:57:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_tiddit     = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_all/main.nf:58:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_tnscope    = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_all/main.nf:61:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi_freebayes  = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_all/main.nf:62:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi_lofreq     = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_all/main.nf:63:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi_manta      = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_all/main.nf:64:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi_mpileup    = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_all/main.nf:65:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi_mutect2    = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_all/main.nf:66:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi_tiddit     = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_all/main.nf:67:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi_tnscope    = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_all/main.nf:221:5`: Variable was declared but not used

  ```nextflow
      vcf_all = Channel.empty()
      ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_all/main.nf:221:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_all = Channel.empty()
                ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_all/main.nf:232:5`: Variable was declared but not used

  ```nextflow
      tbi_all = Channel.empty()
      ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_all/main.nf:232:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi_all = Channel.empty()
                ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_controlfreec/main.nf:26:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_lofreq/main.nf:13:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_lofreq/main.nf:25:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_lofreq/main.nf:26:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_lofreq/main.nf:32:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_lofreq/main.nf:33:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_lofreq/main.nf:43:5`: Variable was declared but not used

  ```nextflow
      vcf = Channel.empty().mix(MERGE_LOFREQ.out.vcf, vcf_branch.no_intervals).map{ meta, vcf -> [ meta - meta.subMap('num_intervals') + [ variantcaller:'lofreq' ], vcf ] }
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_lofreq/main.nf:43:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf = Channel.empty().mix(MERGE_LOFREQ.out.vcf, vcf_branch.no_intervals).map{ meta, vcf -> [ meta - meta.subMap('num_intervals') + [ variantcaller:'lofreq' ], vcf ] }
            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_lofreq/main.nf:44:5`: Variable was declared but not used

  ```nextflow
      tbi = Channel.empty().mix(MERGE_LOFREQ.out.tbi, tbi_branch.no_intervals).map{ meta, tbi -> [ meta - meta.subMap('num_intervals') + [ variantcaller:'lofreq' ], tbi ] }
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_lofreq/main.nf:44:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi = Channel.empty().mix(MERGE_LOFREQ.out.tbi, tbi_branch.no_intervals).map{ meta, tbi -> [ meta - meta.subMap('num_intervals') + [ variantcaller:'lofreq' ], tbi ] }
            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_manta/main.nf:18:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_manta/main.nf:30:5`: Variable was declared but not used

  ```nextflow
      small_indels_vcf = MANTA_TUMORONLY.out.candidate_small_indels_vcf
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_manta/main.nf:31:5`: Variable was declared but not used

  ```nextflow
      candidate_sv_vcf = MANTA_TUMORONLY.out.candidate_sv_vcf
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_manta/main.nf:37:5`: Variable was declared but not used

  ```nextflow
      vcf = tumor_sv_vcf.map{ meta, vcf -> [ meta + [ variantcaller:'manta' ], vcf ] }
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_manta/main.nf:38:5`: Variable was declared but not used

  ```nextflow
      tbi = tumor_sv_vcf_tbi.map{ meta, tbi -> [ meta + [ variantcaller:'manta' ], tbi ] }
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:30:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:34:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      germline_resource_pileup = germline_resource.filter { it != [] }
                                                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:35:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      germline_resource_pileup_tbi = germline_resource_tbi.filter { it != [] }
                                                                    ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:62:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:63:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:68:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:69:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:74:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:75:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:80:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:81:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:94:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf = Channel.empty().mix(MERGE_MUTECT2.out.vcf, vcf_branch.no_intervals).map { meta, vcf -> [meta - meta.subMap('num_intervals'), vcf] }
            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:95:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbi = Channel.empty().mix(MERGE_MUTECT2.out.tbi, tbi_branch.no_intervals).map { meta, tbi -> [meta - meta.subMap('num_intervals'), tbi] }
            ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:96:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      stats = Channel.empty().mix(MERGEMUTECTSTATS.out.stats, stats_branch.no_intervals).map { meta, stats -> [meta - meta.subMap('num_intervals'), stats] }
              ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:97:12`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      f1r2 = Channel.empty().mix(f1r2_to_merge, f1r2_branch.no_intervals).map { meta, f1r2 -> [meta - meta.subMap('num_intervals'), f1r2] }
             ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:109:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:110:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:119:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      pileup_table = Channel.empty().mix(GATHERPILEUPSUMMARIES.out.table, pileup_table_branch.no_intervals).map { meta, table -> [meta - meta.subMap('num_intervals') + [id: meta.sample], table] }
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:125:38`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      calculatecontamination_out_seg = Channel.empty()
                                       ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:126:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      calculatecontamination_out_cont = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:160:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .unique { it[0] }
                    ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:165:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .unique { it[0] }
                    ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_tnscope/main.nf:22:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_tnscope/main.nf:45:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_tnscope/main.nf:46:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_tnscope/main.nf:51:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_tnscope/main.nf:52:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_tnscope/main.nf:63:5`: Variable was declared but not used

  ```nextflow
      vcf   = Channel.empty()
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_tnscope/main.nf:63:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf   = Channel.empty()
              ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_tnscope/main.nf:67:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      index = Channel.empty()
              ^^^^^^^
  ```

- Warning: `subworkflows/local/cram_merge_index_samtools/main.nf:36:5`: Variable was declared but not used

  ```nextflow
      cram_crai = cram_all.join(INDEX_CRAM.out.crai, failOnDuplicate: true, failOnMismatch: true)
      ^^^^^^^^^
  ```

- Warning: `subworkflows/local/cram_qc_mosdepth_samtools/main.nf:17:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/cram_qc_mosdepth_samtools/main.nf:18:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      reports = Channel.empty()
                ^^^^^^^
  ```

- Warning: `subworkflows/local/cram_qc_mosdepth_samtools/main.nf:23:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      MOSDEPTH(cram.combine(intervals.map { meta, bed -> [bed ?: []] }), fasta)
                                            ^^^^
  ```

- Warning: `subworkflows/local/cram_sampleqc/main.nf:14:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/cram_sampleqc/main.nf:15:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      reports = Channel.empty()
                ^^^^^^^
  ```

- Warning: `subworkflows/local/fastq_align/main.nf:40:5`: Variable was declared but not used

  ```nextflow
      bai = SENTIEON_BWAMEM.out.bam_and_bai.map{ meta, _bam_file, bai -> [ meta, bai ] }
      ^^^
  ```

- Warning: `subworkflows/local/post_variantcalling/main.nf:36:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/post_variantcalling/main.nf:37:12`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcfs = Channel.empty()
             ^^^^^^^
  ```

- Warning: `subworkflows/local/post_variantcalling/main.nf:38:12`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tbis = Channel.empty()
             ^^^^^^^
  ```

- Warning: `subworkflows/local/post_variantcalling/main.nf:84:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          all_vcfs = Channel.empty().mix(germline_vcfs, tumor_only_vcfs, somatic_vcfs)
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/post_variantcalling/main.nf:85:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  .branch{ meta, vcf ->
                                                 ^^^
  ```

- Warning: `subworkflows/local/post_variantcalling/main.nf:90:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          all_tbis = Channel.empty().mix(germline_tbis, tumor_only_tbis, somatic_tbis)
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/post_variantcalling/main.nf:91:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                  .branch{ meta, tbi ->
                                                 ^^^
  ```

- Warning: `subworkflows/local/post_variantcalling/main.nf:97:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          all_vcfs.other.subscribe { meta, vcf ->
                                           ^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:57:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:60:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      fasta = fasta_in ? Channel.fromPath(fasta_in).map { fasta -> [[id: fasta.baseName], fasta] }.collect() : Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:60:110`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      fasta = fasta_in ? Channel.fromPath(fasta_in).map { fasta -> [[id: fasta.baseName], fasta] }.collect() : Channel.empty()
                                                                                                               ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:61:5`: Variable was declared but not used

  ```nextflow
      vep_fasta = vep_include_fasta ? fasta : [[id: 'null'], []]
      ^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:70:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              index_alignment = Channel.fromPath(bwa_in).map { index -> [[id: 'bwa'], index] }.collect()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:78:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              index_alignment = Channel.fromPath(bwamem2_in).map { index -> [[id: 'bwamem2'], index] }.collect()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:86:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              index_alignment = Channel.fromPath(dragmap_in).map { index -> [[id: 'dragmap'], index] }.collect()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:90:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          index_alignment = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:99:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          dict = Channel.fromPath(dict_in).map { it -> [[id: 'dict'], it] }.collect()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:102:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          dict = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:111:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          fasta_fai = Channel.fromPath(fasta_fai_in).map { it -> [[id: 'fai'], it] }.collect()
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:114:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          fasta_fai = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:118:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      bbsplit_index = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:127:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  bbsplit_index = Channel.value(file(bbsplit_index_in, checkIfExists: true))
                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:132:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              Channel.from(file(bbsplit_fasta_list_in, checkIfExists: true))
              ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:137:29`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .collect { [it] }
                              ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:150:54`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      bcftools_annotations = bcftools_annotations_in ? Channel.fromPath(bcftools_annotations_in).collect() : Channel.value([])
                                                       ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:150:108`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      bcftools_annotations = bcftools_annotations_in ? Channel.fromPath(bcftools_annotations_in).collect() : Channel.value([])
                                                                                                             ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:151:62`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      bcftools_annotations_tbi = bcftools_annotations_tbi_in ? Channel.fromPath(bcftools_annotations_tbi_in).collect() : Channel.value([])
                                                               ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:151:120`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      bcftools_annotations_tbi = bcftools_annotations_tbi_in ? Channel.fromPath(bcftools_annotations_tbi_in).collect() : Channel.value([])
                                                                                                                         ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:159:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      dbsnp = dbsnp_in ? Channel.fromPath(dbsnp_in).collect() : Channel.value([])
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:159:63`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      dbsnp = dbsnp_in ? Channel.fromPath(dbsnp_in).collect() : Channel.value([])
                                                                ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:160:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      dbsnp_tbi = dbsnp_tbi_in ? Channel.fromPath(dbsnp_tbi_in).collect() : Channel.value([])
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:160:75`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      dbsnp_tbi = dbsnp_tbi_in ? Channel.fromPath(dbsnp_tbi_in).collect() : Channel.value([])
                                                                            ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:168:48`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      germline_resource = germline_resource_in ? Channel.fromPath(germline_resource_in).collect() : Channel.value([])
                                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:168:99`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      germline_resource = germline_resource_in ? Channel.fromPath(germline_resource_in).collect() : Channel.value([])
                                                                                                    ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:169:56`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      germline_resource_tbi = germline_resource_tbi_in ? Channel.fromPath(germline_resource_tbi_in).collect() : Channel.value([])
                                                         ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:169:111`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      germline_resource_tbi = germline_resource_tbi_in ? Channel.fromPath(germline_resource_tbi_in).collect() : Channel.value([])
                                                                                                                ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:177:38`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      known_indels = known_indels_in ? Channel.fromPath(known_indels_in).collect() : Channel.value([])
                                       ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:177:84`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      known_indels = known_indels_in ? Channel.fromPath(known_indels_in).collect() : Channel.value([])
                                                                                     ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:178:46`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      known_indels_tbi = known_indels_tbi_in ? Channel.fromPath(known_indels_tbi_in).collect() : Channel.value([])
                                               ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:178:96`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      known_indels_tbi = known_indels_tbi_in ? Channel.fromPath(known_indels_tbi_in).collect() : Channel.value([])
                                                                                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:186:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      known_snps = known_snps_in ? Channel.fromPath(known_snps_in).collect() : Channel.value([])
                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:186:78`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      known_snps = known_snps_in ? Channel.fromPath(known_snps_in).collect() : Channel.value([])
                                                                               ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:187:42`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      known_snps_tbi = known_snps_tbi_in ? Channel.fromPath(known_snps_tbi_in).collect() : Channel.value([])
                                           ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:187:90`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      known_snps_tbi = known_snps_tbi_in ? Channel.fromPath(known_snps_tbi_in).collect() : Channel.value([])
                                                                                           ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:195:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      pon = pon_in ? Channel.fromPath(pon_in).collect() : Channel.value([])
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:195:57`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      pon = pon_in ? Channel.fromPath(pon_in).collect() : Channel.value([])
                                                          ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:196:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      pon_tbi = pon_tbi_in ? Channel.fromPath(pon_tbi_in).collect() : Channel.value([])
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:196:69`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      pon_tbi = pon_tbi_in ? Channel.fromPath(pon_tbi_in).collect() : Channel.value([])
                                                                      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:206:5`: Variable was declared but not used

  ```nextflow
      known_sites_indels = dbsnp.concat(known_indels).collect()
      ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:207:5`: Variable was declared but not used

  ```nextflow
      known_sites_indels_tbi = dbsnp_tbi.concat(known_indels_tbi).collect()
      ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:208:5`: Variable was declared but not used

  ```nextflow
      known_sites_snps = dbsnp.concat(known_snps).collect()
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:209:5`: Variable was declared but not used

  ```nextflow
      known_sites_snps_tbi = dbsnp_tbi.concat(known_snps_tbi).collect()
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:213:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          UNTAR_MSISENSOR2_MODELS(Channel.fromPath(file(msisensor2_models_in)).map { archive -> [[id: archive.baseName], archive] })
                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:218:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          msisensor2_models = Channel.fromPath(msisensor2_models_in).map { model -> [[id:model.baseName], model] }.collect()
                              ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:221:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          msisensor2_models = Channel.value([])
                              ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:225:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          msisensorpro_scan = Channel.fromPath(msisensorpro_scan_in)
                              ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:233:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          msisensorpro_scan = Channel.value([])
                              ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:238:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ascat_alleles = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:241:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          UNZIP_ALLELES(Channel.fromPath(file(ascat_alleles_in)).map { archive -> [[id: archive.baseName], archive] })
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:246:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ascat_alleles = Channel.fromPath(ascat_alleles_in).collect()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:250:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ascat_loci = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:253:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          UNZIP_LOCI(Channel.fromPath(file(ascat_loci_in)).map { archive -> [[id: archive.baseName], archive] })
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:258:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ascat_loci = Channel.fromPath(ascat_loci_in).collect()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:262:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ascat_loci_gc = Channel.value([])
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:265:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          UNZIP_GC(Channel.fromPath(file(ascat_loci_gc_in)).map { archive -> [[id: archive.baseName], archive] })
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:270:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ascat_loci_gc = Channel.fromPath(ascat_loci_gc_in).collect()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:274:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ascat_loci_rt = Channel.value([])
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:277:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          UNZIP_RT(Channel.fromPath(file(ascat_loci_rt_in)).map { archive -> [[id: archive.baseName], archive] })
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:282:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ascat_loci_rt = Channel.fromPath(ascat_loci_rt_in).collect()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:286:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          chr_dir = Channel.value([])
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:289:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          UNTAR_CHR_DIR(Channel.fromPath(file(chr_dir_in)).map { archive -> [[id: archive.baseName], archive] })
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:294:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          chr_dir = Channel.fromPath(chr_dir_in).collect()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:25:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:27:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      intervals_bed        = Channel.empty() // List of [ bed, num_intervals ], one for each region
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:28:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      intervals_bed_gz_tbi = Channel.empty() // List of [ bed.gz, bed,gz.tbi, num_intervals ], one for each region
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:29:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      intervals_combined   = Channel.empty() // Single bed file containing all intervals
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:36:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          intervals_bed        = Channel.fromPath(file("${outdir}/no_intervals.bed")).map{ it -> [ it, 0 ] }
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:37:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          intervals_bed_gz_tbi = Channel.fromPath(file("${outdir}/no_intervals.bed.{gz,gz.tbi}")).collect().map{ it -> [ it, 0 ] }
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:38:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          intervals_combined   = Channel.fromPath(file("${outdir}/no_intervals.bed")).map{ it -> [ [ id:it.simpleName ], it ] }
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:46:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              CREATE_INTERVALS_BED(intervals_combined.map{ meta, path -> path }, nucleotides_per_second)
                                                           ^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:53:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              intervals_combined = Channel.fromPath(file(intervals)).map{it -> [ [ id:it.baseName ], it ] }
                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:87:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .flatten().collate(2).map{ duration, intervalFile -> intervalFile }.collect()
                                         ^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:93:66`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          TABIX_BGZIPTABIX_INTERVAL_SPLIT(intervals_bed.map{ file, num_intervals -> [ [ id:file.baseName], file ] })
                                                                   ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:95:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          intervals_bed_gz_tbi = TABIX_BGZIPTABIX_INTERVAL_SPLIT.out.gz_index.map{ meta, bed, tbi -> [ bed, tbi ] }.toList()
                                                                                   ^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:103:5`: Variable was declared but not used

  ```nextflow
      intervals_bed_combined        = intervals_combined.map{meta, bed -> bed }.collect()
      ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:103:60`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      intervals_bed_combined        = intervals_combined.map{meta, bed -> bed }.collect()
                                                             ^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:104:5`: Variable was declared but not used

  ```nextflow
      intervals_bed_gz_tbi_combined = TABIX_BGZIPTABIX_INTERVAL_COMBINED.out.gz_index.map{meta, gz, tbi -> [gz, tbi] }.collect()
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:104:89`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      intervals_bed_gz_tbi_combined = TABIX_BGZIPTABIX_INTERVAL_COMBINED.out.gz_index.map{meta, gz, tbi -> [gz, tbi] }.collect()
                                                                                          ^^^^
  ```

- Warning: `subworkflows/local/prepare_reference_cnvkit/main.nf:10:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:16:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          has_vardb: it.vardb != null
                     ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:23:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_branched.needs_vardb.map { [[id: it.vcf.baseName], it.vcf, it.tbi, it.fields ? it.fields.replace(';', ',') : ''] }
                                              ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:23:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_branched.needs_vardb.map { [[id: it.vcf.baseName], it.vcf, it.tbi, it.fields ? it.fields.replace(';', ',') : ''] }
                                                                ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:23:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_branched.needs_vardb.map { [[id: it.vcf.baseName], it.vcf, it.tbi, it.fields ? it.fields.replace(';', ',') : ''] }
                                                                        ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:23:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_branched.needs_vardb.map { [[id: it.vcf.baseName], it.vcf, it.tbi, it.fields ? it.fields.replace(';', ',') : ''] }
                                                                                ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:23:91`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_branched.needs_vardb.map { [[id: it.vcf.baseName], it.vcf, it.tbi, it.fields ? it.fields.replace(';', ',') : ''] }
                                                                                            ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:29:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .join(ch_branched.needs_vardb.map { [it.vcf.baseName, it] })
                                               ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:29:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .join(ch_branched.needs_vardb.map { [it.vcf.baseName, it] })
                                                                ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:34:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [it.vcf, it.tbi, it.vardb, it.fields ? it.fields.replace(';', ',') : '', it.prefix ?: ''] }
                  ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:34:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [it.vcf, it.tbi, it.vardb, it.fields ? it.fields.replace(';', ',') : '', it.prefix ?: ''] }
                          ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:34:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [it.vcf, it.tbi, it.vardb, it.fields ? it.fields.replace(';', ',') : '', it.prefix ?: ''] }
                                  ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:34:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [it.vcf, it.tbi, it.vardb, it.fields ? it.fields.replace(';', ',') : '', it.prefix ?: ''] }
                                            ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:34:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [it.vcf, it.tbi, it.vardb, it.fields ? it.fields.replace(';', ',') : '', it.prefix ?: ''] }
                                                        ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:34:89`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [it.vcf, it.tbi, it.vardb, it.fields ? it.fields.replace(';', ',') : '', it.prefix ?: ''] }
                                                                                          ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:42:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  list.collect { it[0] },  // db_vcf
                                 ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:43:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  list.collect { it[1] },  // db_vcf_tbi
                                 ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:44:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  list.collect { it[2] },  // db_vardb
                                 ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:45:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  list.collect { it[3] },  // db_fields
                                 ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:46:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  list.collect { it[4] }   // db_prefixes
                                 ^^
  ```

- Warning: `subworkflows/local/samplesheet_to_channel/main.nf:13:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      bcftools_columns              // Path: bcftools columns
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/samplesheet_to_channel/main.nf:53:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def status0_count = samples.count { it.status == 0 }
                                                  ^^
  ```

- Warning: `subworkflows/local/samplesheet_to_channel/main.nf:54:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def status1_count = samples.count { it.status == 1 }
                                                  ^^
  ```

- Warning: `subworkflows/local/samplesheet_to_channel/main.nf:70:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { combination_key, combination_list ->
                 ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/samplesheet_to_channel/main.nf:90:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              [patient, samples.collect { it.sample }]
                                          ^^
  ```

- Warning: `subworkflows/local/samplesheet_to_channel/main.nf:245:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter { it[0].status == 1 }
                        ^^
  ```

- Warning: `subworkflows/local/samplesheet_to_channel/main.nf:263:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter { it[0].status == 0 }
                        ^^
  ```

- Warning: `subworkflows/local/samplesheet_to_channel/main.nf:437:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              if (it[0].sex == 'NA') {
                  ^^
  ```

- Warning: `subworkflows/local/samplesheet_to_channel/main.nf:446:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              if (it[0].status == 1 && !it[0].containsKey('contamination')) {
                  ^^
  ```

- Warning: `subworkflows/local/samplesheet_to_channel/main.nf:446:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              if (it[0].status == 1 && !it[0].containsKey('contamination')) {
                                        ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_sarek_pipeline/main.nf:38:5`: Variable was declared but not used

  ```nextflow
      versions = channel.empty()
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:15:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:18:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch{ meta, vcf, tbi ->
                         ^^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:18:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch{ meta, vcf, tbi ->
                              ^^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:54:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                              def sorted_vcfs = sorted_pairs.collect { it[0] }
                                                                       ^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:55:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                              def callers = sorted_pairs.collect { it[1] }
                                                                   ^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:65:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, dir ->
                    ^^^^
  ```

- Warning: `subworkflows/local/vcf_qc_bcftools_vcftools/main.nf:13:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_variant_filtering_gatk/main.nf:17:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_variant_filtering_gatk/main.nf:26:5`: Variable was declared but not used

  ```nextflow
      filtered_vcf = FILTERVARIANTTRANCHES.out.vcf
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_variant_filtering_gatk/main.nf:30:5`: Variable was declared but not used

  ```nextflow
      filtered_tbi = FILTERVARIANTTRANCHES.out.tbi
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_ngscheckmate/main.nf:13:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```

- Warning: `workflows/sarek/main.nf:141:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              bam: it[0].data_type == "bam"
                   ^^
  ```

- Warning: `workflows/sarek/main.nf:142:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              fastq_gz: it[0].data_type == "fastq_gz"
                        ^^
  ```

- Warning: `workflows/sarek/main.nf:143:34`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              one_fastq_gz_spring: it[0].data_type == "one_fastq_gz_spring"
                                   ^^
  ```

- Warning: `workflows/sarek/main.nf:144:34`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              two_fastq_gz_spring: it[0].data_type == "two_fastq_gz_spring"
                                   ^^
  ```

- Warning: `workflows/sarek/main.nf:291:77`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              cram_variant_calling_status_tmp = cram_variant_calling.branch { meta, file, index ->
                                                                              ^^^^
  ```

- Warning: `workflows/sarek/main.nf:291:89`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              cram_variant_calling_status_tmp = cram_variant_calling.branch { meta, file, index ->
                                                                                          ^^^^^
  ```

- Warning: `workflows/sarek/main.nf:311:75`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          cram_variant_calling_status = cram_variant_calling.branch { meta, file, index ->
                                                                            ^^^^
  ```

- Warning: `workflows/sarek/main.nf:311:81`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          cram_variant_calling_status = cram_variant_calling.branch { meta, file, index ->
                                                                                  ^^^^^
  ```

- Warning: `workflows/sarek/main.nf:317:73`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          bam_variant_calling_status = bam_variant_calling.branch { meta, file, index ->
                                                                          ^^^^
  ```

- Warning: `workflows/sarek/main.nf:317:79`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          bam_variant_calling_status = bam_variant_calling.branch { meta, file, index ->
                                                                                ^^^^^
  ```

- Warning: `workflows/sarek/main.nf:703:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def InputStream gzipStream = new java.util.zip.GZIPInputStream(it)
                                                                             ^^
  ```
