# Nextflow lint results

- Generated: 2026-06-16T14:25:48.653424254Z
- Nextflow version: 26.04.3
- Summary: 7 errors, 120 warnings

## :x: Errors

- Error: `conf/modules.config:282:17`: Unexpected input: ':'

  ```nextflow
          withName: '.*:SOMATIC_SV:TABIX_SV_VCF' {
                  ^
  ```

- Error: `nextflow.config:350:34`: `manifest` is not defined

  ```nextflow
  \033[0;35m  nf-core/pacsomatic ${manifest.version}\033[0m
                                   ^^^^^^^^
  ```

- Error: `nextflow.config:353:26`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                           ^^^^^^^^
  ```

- Error: `nextflow.config:353:69`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                      ^^^^^^^^
  ```

- Error: `nextflow.config:353:186`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                                                                                                                                           ^^^^^^^^
  ```

- Error: `nextflow.config:362:22`: `validation` is not defined

  ```nextflow
          beforeText = validation.help.beforeText
                       ^^^^^^^^^^
  ```

- Error: `nextflow.config:363:21`: `validation` is not defined

  ```nextflow
          afterText = validation.help.afterText
                      ^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `main.nf:55:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = PACSOMATIC.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/annotatr_dmr/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/annotatr_dmr/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/dss_dmr/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/dss_dmr/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/purple/main.nf:32:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/purple/main.nf:87:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/bcftools/concat/main.nf:32:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input = vcfs.sort{it.toString()}.join(" ")
                            ^^
  ```

- Warning: `modules/nf-core/bcftools/index/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/bcftools/index/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
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

- Warning: `modules/nf-core/clair3/main.nf:72:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/gunzip/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/pbmm2/align/main.nf:41:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/pbtk/pbmerge/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/severus/main.nf:59:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `nextflow.config:353:129`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                                                                                  ^^
  ```

- Warning: `subworkflows/local/cnv_calling/main.nf:19:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/germline_calling_phasing/main.nf:17:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/germline_calling_phasing/main.nf:53:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_phased_bam_bai = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/germline_calling_phasing/main.nf:54:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_phased_vcf_tbi = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/germline_calling_phasing/main.nf:73:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .multiMap { meta_id, meta, vcf, tbi, meta2, bam, bai ->
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/methylation_analysis/main.nf:19:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/methylation_analysis/main.nf:49:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_dmr_tsv = Channel.empty()
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/methylation_analysis/main.nf:50:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_dmr_annotated = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/methylation_analysis/main.nf:56:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { patient_normal_id, pair_meta, tumor_bed, normal_meta, normal_bed ->
                     ^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/methylation_analysis/main.nf:56:61`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { patient_normal_id, pair_meta, tumor_bed, normal_meta, normal_bed ->
                                                              ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome.nf:17:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome.nf:22:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_genome_fasta = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome.nf:23:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_genome_fai = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/signature_analysis/main.nf:21:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/signature_analysis/main.nf:26:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_chord_mutation = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/signature_analysis/main.nf:27:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_chord_prediction = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/signature_analysis/main.nf:84:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_mutational_signature = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/somatic_snv_indel/main.nf:24:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/somatic_snv_indel/main.nf:44:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_vep_vcf = Channel.empty()
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/somatic_snv_indel/main.nf:45:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_vep_tab = Channel.empty()
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/somatic_snv_indel/main.nf:56:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ch_vep_download = Channel.value(
                                    ^^^^^^^
  ```

- Warning: `subworkflows/local/somatic_snv_indel/main.nf:64:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      .map { meta, path_prefix -> [path_prefix] }
                             ^^^^
  ```

- Warning: `subworkflows/local/somatic_snv_indel/main.nf:89:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_germline_phased_bam_bai = Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/somatic_snv_indel/main.nf:91:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_germline_phased_vcf     = Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/somatic_snv_indel/main.nf:92:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_somatic_phased_vcf      = Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/somatic_snv_indel/main.nf:119:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .multiMap { meta_id, meta, vcf, tbi, meta2, bam, bai, meta3, somatic_vcf, somatic_tbi ->
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/somatic_snv_indel/main.nf:119:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .multiMap { meta_id, meta, vcf, tbi, meta2, bam, bai, meta3, somatic_vcf, somatic_tbi ->
                                   ^^^^
  ```

- Warning: `subworkflows/local/somatic_snv_indel/main.nf:119:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .multiMap { meta_id, meta, vcf, tbi, meta2, bam, bai, meta3, somatic_vcf, somatic_tbi ->
                                                   ^^^^^
  ```

- Warning: `subworkflows/local/somatic_sv/main.nf:24:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/somatic_sv/main.nf:64:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_annotsv_tsv = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/svpack_annotate/main.nf:22:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/tumor_clonality/main.nf:26:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/tumor_clonality/main.nf:38:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def missing_params = required_params.findAll { !params[it] }
                                                            ^^
  ```

- Warning: `subworkflows/local/tumor_clonality/main.nf:66:5`: Variable was declared but not used

  ```nextflow
      ch_amber_dir = AMBER.out.amber_dir
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/tumor_clonality/main.nf:91:5`: Variable was declared but not used

  ```nextflow
      ch_cobalt_dir = COBALT.out.cobalt_dir
      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pacsomatic_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pacsomatic_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pacsomatic_pipeline/main.nf:39:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pacsomatic_pipeline/main.nf:84:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_pacsomatic_pipeline/main.nf:95:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              } catch (Exception e) {
                                 ^
  ```

- Warning: `subworkflows/nf-core/bam_sort_stats_samtools/main.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_stats_samtools/main.nf:15:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
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

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:44:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:50:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:51:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:52:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_report = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:59:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ? Channel.value([[:], file(params.severus_trf_bed, checkIfExists: true)])
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:60:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.value([[:], []])
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:63:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ? Channel.value([[:], file(params.svpack_ctrl_vcf, checkIfExists: true)])
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:64:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.value([[:], []])
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:67:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ? Channel.value([[:], file(params.svpack_ref_gff, checkIfExists: true)])
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:68:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.value([[:], []])
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:71:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ? Channel.value([[:], file(params.annotsv_cache, checkIfExists: true)])
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:72:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.empty()
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:76:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ? Channel.value([[:], file(params.cnv_target_bed, checkIfExists: true)])
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:77:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.value([[:], []])
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:80:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ? Channel.value([[:], file(params.cnv_reference, checkIfExists: true)])
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:81:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.value([[:], []])
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:84:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ? Channel.value(file(params.cnv_germline_vcf, checkIfExists: true))
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:85:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.value([[]])
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:89:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ? Channel.value(file(params.target_regions_bed, checkIfExists: true))
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:90:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.value([])
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:93:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ? Channel.value(file(params.heterozygous_sites, checkIfExists: true))
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:94:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.value([])
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:97:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ? Channel.value(file(params.diploid_regions, checkIfExists: true))
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:98:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.value([])
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:101:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ? Channel.value(file(params.target_region_normalisation, checkIfExists: true))
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:102:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.value([])
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:105:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ? Channel.value(file(params.gc_profile, checkIfExists: true))
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:106:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.value([])
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:110:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ? Channel.value(file(params.known_hotspots_somatic, checkIfExists: true))
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:111:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.value([])
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:114:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ? Channel.value(file(params.known_hotspots_germline, checkIfExists: true))
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:115:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.value([])
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:118:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ? Channel.value(file(params.driver_gene_panel, checkIfExists: true))
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:119:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.value([])
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:122:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ? Channel.value(file(params.ensembl_data_dir, checkIfExists: true, type: 'dir'))
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:123:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.value([])
            ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:194:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_mosdepth_multiqc_files = Channel.empty()
                                  ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:212:35`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_genome_fasta.map { it[1] },
                                    ^^
  ```

- Warning: `workflows/pacsomatic.nf:213:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_genome_fai.map { it[1] },
                                  ^^
  ```

- Warning: `workflows/pacsomatic.nf:281:5`: Variable was declared but not used

  ```nextflow
      ch_vcf_normals = ch_vcf_normals_tmp
      ^^^^^^^^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:282:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { patient, meta, vcf, tbi ->
                 ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:287:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { patient, meta, vcf, tbi ->
                 ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:294:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_somatic_snv_vcf_gz = Channel.empty()
                              ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:295:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_somatic_phased_bam = Channel.empty()
                              ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:317:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_somatic_sv_vcf = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:418:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_multiqc_config        = Channel.fromPath(
                                     ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:421:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              Channel.fromPath(params.multiqc_config, checkIfExists: true) :
              ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:422:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              Channel.empty()
              ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:424:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              Channel.fromPath(params.multiqc_logo, checkIfExists: true) :
              ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:425:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              Channel.empty()
              ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:429:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_workflow_summary = Channel.value(paramsSummaryMultiqc(summary_params))
                                ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:435:49`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_methods_description                = Channel.value(
                                                  ^^^^^^^
  ```

- Warning: `workflows/pacsomatic.nf:447:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(ch_ordered_stats.collect{it[1]}.ifEmpty([]))
                                                                           ^^
  ```

- Warning: `workflows/pacsomatic.nf:448:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(ch_ordered_flagstat.collect{it[1]}.ifEmpty([]))
                                                                              ^^
  ```

- Warning: `workflows/pacsomatic.nf:449:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(ch_ordered_idxstats.collect{it[1]}.ifEmpty([]))
                                                                              ^^
  ```

- Warning: `workflows/pacsomatic.nf:450:83`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(ch_mosdepth_multiqc_files.collect{it[1]}.ifEmpty([]))
                                                                                    ^^
  ```
