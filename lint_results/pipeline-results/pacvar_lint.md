# Nextflow lint results

- Generated: 2026-03-12T00:18:00.238086688Z
- Nextflow version: 26.02.0-edge
- Summary: 6 errors, 29 warnings

## :x: Errors

- Error: `modules/nf-core/deepvariant/main.nf:1:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  def deprecation_message = """
  ^^^
  ```

- Error: `modules/nf-core/deepvariant/main.nf:29:30`: `prefix` is not defined

  ```nextflow
      tuple val(meta), path("${prefix}.vcf.gz")      ,  emit: vcf
                               ^^^^^^
  ```

- Error: `modules/nf-core/deepvariant/main.nf:30:30`: `prefix` is not defined

  ```nextflow
      tuple val(meta), path("${prefix}.vcf.gz.tbi")  ,  emit: vcf_tbi
                               ^^^^^^
  ```

- Error: `modules/nf-core/deepvariant/main.nf:31:30`: `prefix` is not defined

  ```nextflow
      tuple val(meta), path("${prefix}.g.vcf.gz")    ,  emit: gvcf
                               ^^^^^^
  ```

- Error: `modules/nf-core/deepvariant/main.nf:32:30`: `prefix` is not defined

  ```nextflow
      tuple val(meta), path("${prefix}.g.vcf.gz.tbi"),  emit: gvcf_tbi
                               ^^^^^^
  ```

- Error: `modules/nf-core/deepvariant/main.nf:39:19`: `deprecation_message` is not defined

  ```nextflow
      assert false: deprecation_message
                    ^^^^^^^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `main.nf:81:86`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      dbsnp                = params.dbsnp ? channel.fromPath(params.dbsnp).collect() : Channel.value([])
                                                                                       ^^^^^^^
  ```

- Warning: `main.nf:82:94`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      dbsnp_tbi            = params.dbsnp_tbi ? channel.fromPath(params.dbsnp_tbi).collect() : Channel.value([])
                                                                                               ^^^^^^^
  ```

- Warning: `modules/nf-core/deepvariant/main.nf:1:5`: Variable was declared but not used

  ```nextflow
  def deprecation_message = """
      ^^^^^^^^^^^^^^^^^^^
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

- Warning: `modules/nf-core/pbsv/call/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/pbsv/discover/main.nf:36:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/pbtk/pbmerge/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/trgt/genotype/main.nf:45:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/trgt/plot/main.nf:67:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/bam_snp_variant_calling/main.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_snp_variant_calling/main.nf:18:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      intervals_path = intervals.map{metadata, interval -> [interval]}
                                     ^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_sv_variant_calling/main.nf:15:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      fasta_fai               // tuple val(meta), path(fai)
      ^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_sv_variant_calling/main.nf:65:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_discover_bam_bai.map { meta, discover_dir, bam, bai -> [meta, discover_dir] },
                                                            ^^^
  ```

- Warning: `subworkflows/local/bam_sv_variant_calling/main.nf:65:64`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_discover_bam_bai.map { meta, discover_dir, bam, bai -> [meta, discover_dir] },
                                                                 ^^^
  ```

- Warning: `subworkflows/local/bam_sv_variant_calling/main.nf:67:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_discover_bam_bai.map { meta, discover_dir, bam, bai -> [meta, bam, bai] },
                                              ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/set_value_channel/main.nf:13:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel // Prepare value channel
      ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pacvar_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pacvar_pipeline/main.nf:37:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pacvar_pipeline/main.nf:110:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, bam, pbi, fail ->
                         ^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pacvar_pipeline/main.nf:150:9`: Variable was declared but not used

  ```nextflow
      def multiqc_reports = multiqc_report.toList()
          ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/pacvar.nf:67:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_barcode = Channel.value(file(params.barcodes))
                       ^^^^^^^
  ```

- Warning: `workflows/pacvar.nf:91:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      pbmm2_input_filter_ch = pbmm2_input_ch.filter { meta, bam ->
                                                            ^^^
  ```

- Warning: `workflows/pacvar.nf:118:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, bams -> bams.size() > 1 }
                        ^^^^
  ```

- Warning: `workflows/pacvar.nf:123:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, bams -> bams.size() == 1 }
                        ^^^^
  ```

- Warning: `workflows/pacvar.nf:143:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ordered_bam_ch = bam_bai_ch.map { meta, bam, bai -> [meta, bam] }
                                                   ^^^
  ```

- Warning: `workflows/pacvar.nf:144:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ordered_bai_ch = bam_bai_ch.map { meta, bam, bai -> [meta, bai] }
                                              ^^^
  ```

- Warning: `workflows/pacvar.nf:197:90`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  cnv_input_bam_bai_maf_ch = bam_bai_vcf_snp_ch.map { meta, bam, bai, vcf, tbi ->
                                                                                           ^^^
  ```

- Warning: `workflows/pacvar.nf:222:122`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  (sv_input_bam_ch, sv_input_bai_ch, sv_input_maf_ch) = bam_bai_vcf_snp_ch.multiMap { meta, bam, bai, vcf, tbi ->
                                                                                                                           ^^^
  ```
