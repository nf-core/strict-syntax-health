# Nextflow lint results

- Generated: 2026-06-16T14:37:50.050404382Z
- Nextflow version: 26.04.3
- Summary: 56 warnings

## :warning: Warnings

- Warning: `conf/modules.config:39:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .findAll { it }
                     ^^
  ```

- Warning: `main.nf:44:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `main.nf:45:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      fasta = params.fasta ? Channel.fromPath(params.fasta).map{ it -> [ [id:it.baseName], it ] }.collect() : Channel.empty()
                             ^^^^^^^
  ```

- Warning: `main.nf:45:109`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      fasta = params.fasta ? Channel.fromPath(params.fasta).map{ it -> [ [id:it.baseName], it ] }.collect() : Channel.empty()
                                                                                                              ^^^^^^^
  ```

- Warning: `main.nf:46:45`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      drivers_table =  params.drivers_table ? Channel.fromPath(params.drivers_table).map{ it -> [ it ] }.collect() : Channel.empty()
                                              ^^^^^^^
  ```

- Warning: `main.nf:46:116`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      drivers_table =  params.drivers_table ? Channel.fromPath(params.drivers_table).map{ it -> [ it ] }.collect() : Channel.empty()
                                                                                                                     ^^^^^^^
  ```

- Warning: `main.nf:49:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ensemblvep_info = Channel.of([ [ id:"${params.vep_cache_version}_${params.vep_genome}" ], params.vep_genome, params.vep_species, params.vep_cache_version ])
                            ^^^^^^^
  ```

- Warning: `main.nf:51:66`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          vep_cache = ENSEMBLVEP_DOWNLOAD.out.cache.collect().map{ meta, cache -> [ cache ] }
                                                                   ^^^^
  ```

- Warning: `main.nf:55:46`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              def vep_tar = params.vep_cache ? Channel.fromPath(params.vep_cache).map{ it -> [ [id:it.baseName], it ] }.collect() : Channel.empty()
                                               ^^^^^^^
  ```

- Warning: `main.nf:55:131`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              def vep_tar = params.vep_cache ? Channel.fromPath(params.vep_cache).map{ it -> [ [id:it.baseName], it ] }.collect() : Channel.empty()
                                                                                                                                    ^^^^^^^
  ```

- Warning: `main.nf:57:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              vep_cache = UNTAR.out.untar.map{meta, cache_path ->
                                              ^^^^
  ```

- Warning: `main.nf:83:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions = ch_versions
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `main.nf:96:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
        ? Channel.fromList(samplesheetToList(params.input, "assets/schema_input.json"))
          ^^^^^^^
  ```

- Warning: `main.nf:97:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
        : Channel.empty()
          ^^^^^^^
  ```

- Warning: `modules/local/annotate_driver/main.nf:19:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args   ?: ""
          ^^^^
  ```

- Warning: `modules/local/get_positions/main.nf:19:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args   ?: ""
          ^^^^
  ```

- Warning: `modules/local/get_positions/main_rel.nf:19:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args   ?: ""
          ^^^^
  ```

- Warning: `modules/local/get_positions/main_rel.nf:20:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/join_positions/main.nf:19:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/sigprofiler/main.nf:26:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args   ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/sigprofiler/main.nf:36:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def signatures = context_types.collect { context_map[it] }
                                                          ^^
  ```

- Warning: `subworkflows/local/annotation_cache_initialisation/main.nf:22:5`: Variable was declared but not used

  ```nextflow
      ensemblvep_cache = Channel.fromPath(file("${vep_cache}/${vep_annotation_cache_key}"), checkIfExists: true).collect()
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/annotation_cache_initialisation/main.nf:22:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ensemblvep_cache = Channel.fromPath(file("${vep_cache}/${vep_annotation_cache_key}"), checkIfExists: true).collect()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/annotation_cache_initialisation/main.nf:25:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      ensemblvep_cache
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/formatter/main.nf:16:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_versions = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/lifter/main.nf:36:70`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          def all_pos = GET_POSITIONS_ALL.out.all_pos.transpose().map{ meta, _rds ->
                                                                       ^^^^
  ```

- Warning: `subworkflows/local/qc/main.nf:15:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_versions = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/signature_deconvolution/main.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/signature_deconvolution/main.nf:30:88`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          input_sparsesig = FORMATTER_RDS_SPARSESIGNATURES.out.out_data.map { meta, tsv, sample ->
                                                                                         ^^^^^^
  ```

- Warning: `subworkflows/local/signature_deconvolution/main.nf:57:85`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          input_sigprofiler = FORMATTER_RDS_SIGPROFILER.out.out_data.map { meta, tsv, sample ->
                                                                                      ^^^^^^
  ```

- Warning: `subworkflows/local/subclonal_deconvolution/main.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_tumourevo_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_tumourevo_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
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

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:72:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/tumourevo.nf:42:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { id, meta, vcf, tbi, bam, bai, cna_segs, cna_extra, n  ->
                     ^^
  ```

- Warning: `workflows/tumourevo.nf:51:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input_vcf = input.map{ meta, vcf, tbi, bam, bai, cna_segs, cna_extra  ->
                                             ^^^
  ```

- Warning: `workflows/tumourevo.nf:51:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input_vcf = input.map{ meta, vcf, tbi, bam, bai, cna_segs, cna_extra  ->
                                                  ^^^
  ```

- Warning: `workflows/tumourevo.nf:51:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input_vcf = input.map{ meta, vcf, tbi, bam, bai, cna_segs, cna_extra  ->
                                                       ^^^^^^^^
  ```

- Warning: `workflows/tumourevo.nf:51:64`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input_vcf = input.map{ meta, vcf, tbi, bam, bai, cna_segs, cna_extra  ->
                                                                 ^^^^^^^^^
  ```

- Warning: `workflows/tumourevo.nf:55:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input_cna = input.map{ meta, vcf, tbi, bam, bai, cna_segs, cna_extra  ->
                                   ^^^
  ```

- Warning: `workflows/tumourevo.nf:55:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input_cna = input.map{ meta, vcf, tbi, bam, bai, cna_segs, cna_extra  ->
                                        ^^^
  ```

- Warning: `workflows/tumourevo.nf:55:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input_cna = input.map{ meta, vcf, tbi, bam, bai, cna_segs, cna_extra  ->
                                             ^^^
  ```

- Warning: `workflows/tumourevo.nf:55:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input_cna = input.map{ meta, vcf, tbi, bam, bai, cna_segs, cna_extra  ->
                                                  ^^^
  ```

- Warning: `workflows/tumourevo.nf:59:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input_bam = input.map{ meta, vcf, tbi, bam, bai, cna_segs, cna_extra  ->
                                   ^^^
  ```

- Warning: `workflows/tumourevo.nf:59:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input_bam = input.map{ meta, vcf, tbi, bam, bai, cna_segs, cna_extra  ->
                                        ^^^
  ```

- Warning: `workflows/tumourevo.nf:59:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input_bam = input.map{ meta, vcf, tbi, bam, bai, cna_segs, cna_extra  ->
                                                       ^^^^^^^^
  ```

- Warning: `workflows/tumourevo.nf:59:64`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input_bam = input.map{ meta, vcf, tbi, bam, bai, cna_segs, cna_extra  ->
                                                                 ^^^^^^^^^
  ```

- Warning: `workflows/tumourevo.nf:93:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch { meta, rds, bam, bai ->
                              ^^^
  ```

- Warning: `workflows/tumourevo.nf:93:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch { meta, rds, bam, bai ->
                                   ^^^
  ```

- Warning: `workflows/tumourevo.nf:93:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch { meta, rds, bam, bai ->
                                        ^^^
  ```

- Warning: `workflows/tumourevo.nf:102:56`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      rds_input = join_input.multisample.map{ meta, rds, bam, bai ->
                                                         ^^^
  ```

- Warning: `workflows/tumourevo.nf:102:61`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      rds_input = join_input.multisample.map{ meta, rds, bam, bai ->
                                                              ^^^
  ```

- Warning: `workflows/tumourevo.nf:131:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions = ch_collated_versions
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```
