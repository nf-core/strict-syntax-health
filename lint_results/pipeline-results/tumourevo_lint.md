# Nextflow lint results

- Generated: 2026-04-03T00:28:18.777144852Z
- Nextflow version: 26.03.1-edge
- Summary: 9 errors, 60 warnings

## :x: Errors

- Error: `main.nf:35:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  input = params.input ? Channel.fromList(samplesheetToList(params.input, "assets/schema_input.json")) : Channel.empty()
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:65:51`: `path` is already declared

  ```nextflow
              vep_cache = UNTAR.out.untar.map{meta, path ->
                                                    ^^^^
  ```

- Error: `main.nf:107:9`: `input` is not defined

  ```nextflow
          input
          ^^^^^
  ```

- Error: `subworkflows/local/lifter/main.nf:24:36`: `bam` is already declared

  ```nextflow
          rds = data.map{ meta, rds, bam, bai ->
                                     ^^^
  ```

- Error: `subworkflows/local/lifter/main.nf:28:35`: `rds` is already declared

  ```nextflow
          all_rds = data.map{ meta, rds, bam, bai ->
                                    ^^^
  ```

- Error: `subworkflows/local/lifter/main.nf:28:40`: `bam` is already declared

  ```nextflow
          all_rds = data.map{ meta, rds, bam, bai ->
                                         ^^^
  ```

- Error: `subworkflows/local/lifter/main.nf:35:72`: `rds` is already declared

  ```nextflow
          all_pos = GET_POSITIONS_ALL.out.all_pos.transpose().map{ meta, rds ->
                                                                         ^^^
  ```

- Error: `workflows/tumourevo.nf:39:17`: Variables in a closure should be declared with `def`

  ```nextflow
                  n = vcf.baseName.unique().size()
                  ^
  ```

- Error: `workflows/tumourevo.nf:42:71`: `n` is already declared

  ```nextflow
              .map { id, meta, vcf, tbi, bam, bai, cna_segs, cna_extra, n  ->
                                                                        ^
  ```

## :warning: Warnings

- Warning: `conf/modules.config:39:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .findAll { it }
                     ^^
  ```

- Warning: `main.nf:35:1`: Variable was declared but not used

  ```nextflow
  input = params.input ? Channel.fromList(samplesheetToList(params.input, "assets/schema_input.json")) : Channel.empty()
  ^^^^^
  ```

- Warning: `main.nf:35:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  input = params.input ? Channel.fromList(samplesheetToList(params.input, "assets/schema_input.json")) : Channel.empty()
                         ^^^^^^^
  ```

- Warning: `main.nf:35:104`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
  input = params.input ? Channel.fromList(samplesheetToList(params.input, "assets/schema_input.json")) : Channel.empty()
                                                                                                         ^^^^^^^
  ```

- Warning: `main.nf:52:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `main.nf:53:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      fasta = params.fasta ? Channel.fromPath(params.fasta).map{ it -> [ [id:it.baseName], it ] }.collect() : Channel.empty()
                             ^^^^^^^
  ```

- Warning: `main.nf:53:109`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      fasta = params.fasta ? Channel.fromPath(params.fasta).map{ it -> [ [id:it.baseName], it ] }.collect() : Channel.empty()
                                                                                                              ^^^^^^^
  ```

- Warning: `main.nf:54:45`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      drivers_table =  params.drivers_table ? Channel.fromPath(params.drivers_table).map{ it -> [ it ] }.collect() : Channel.empty()
                                              ^^^^^^^
  ```

- Warning: `main.nf:54:116`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      drivers_table =  params.drivers_table ? Channel.fromPath(params.drivers_table).map{ it -> [ it ] }.collect() : Channel.empty()
                                                                                                                     ^^^^^^^
  ```

- Warning: `main.nf:57:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ensemblvep_info = Channel.of([ [ id:"${params.vep_cache_version}_${params.vep_genome}" ], params.vep_genome, params.vep_species, params.vep_cache_version ])
                            ^^^^^^^
  ```

- Warning: `main.nf:59:66`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          vep_cache = ENSEMBLVEP_DOWNLOAD.out.cache.collect().map{ meta, cache -> [ cache ] }
                                                                   ^^^^
  ```

- Warning: `main.nf:63:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              path = params.vep_cache ? Channel.fromPath(params.vep_cache).map{ it -> [ [id:it.baseName], it ] }.collect() : Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `main.nf:63:124`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              path = params.vep_cache ? Channel.fromPath(params.vep_cache).map{ it -> [ [id:it.baseName], it ] }.collect() : Channel.empty()
                                                                                                                             ^^^^^^^
  ```

- Warning: `main.nf:65:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              vep_cache = UNTAR.out.untar.map{meta, path ->
                                              ^^^^
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

- Warning: `modules/nf-core/cnaqc/main.nf:25:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/cnaqc/main.nf:26:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/cnaqc/main.nf:31:9`: Variable was declared but not used

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

- Warning: `subworkflows/local/annotation_cache_initialisation/main.nf:22:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ensemblvep_cache = Channel.fromPath(file("${vep_cache}/${vep_annotation_cache_key}"), checkIfExists: true).collect()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/formatter/main.nf:16:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_versions = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/lifter/main.nf:17:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          out = Channel.empty()
                ^^^^^^^
  ```

- Warning: `subworkflows/local/lifter/main.nf:18:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_versions = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/lifter/main.nf:20:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          bam = data.map{ meta, rds, bam, bai ->
                                ^^^
  ```

- Warning: `subworkflows/local/lifter/main.nf:20:41`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          bam = data.map{ meta, rds, bam, bai ->
                                          ^^^
  ```

- Warning: `subworkflows/local/lifter/main.nf:24:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          rds = data.map{ meta, rds, bam, bai ->
                                     ^^^
  ```

- Warning: `subworkflows/local/lifter/main.nf:24:41`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          rds = data.map{ meta, rds, bam, bai ->
                                          ^^^
  ```

- Warning: `subworkflows/local/lifter/main.nf:28:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          all_rds = data.map{ meta, rds, bam, bai ->
                                         ^^^
  ```

- Warning: `subworkflows/local/lifter/main.nf:28:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          all_rds = data.map{ meta, rds, bam, bai ->
                                              ^^^
  ```

- Warning: `subworkflows/local/lifter/main.nf:35:66`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          all_pos = GET_POSITIONS_ALL.out.all_pos.transpose().map{ meta, rds ->
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
