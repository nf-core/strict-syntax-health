# Nextflow lint results

- Generated: 2026-06-16T20:32:59.522777708Z
- Nextflow version: 26.04.3
- Summary: 6 errors, 34 warnings

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

- Warning: `main.nf:115:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = PACVAR.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
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

- Warning: `subworkflows/local/repeat_characterization/main.nf:32:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta_fasta, fasta_file, meta_fai, fai_file -> [meta_fasta, fasta_file, fai_file] }
                                         ^^^^^^^^
  ```

- Warning: `subworkflows/local/repeat_characterization/main.nf:64:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions       = ch_versions
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/set_value_channel/main.nf:15:16`: Variable was declared but not used

  ```nextflow
          .set { data }
                 ^^^^
  ```

- Warning: `subworkflows/local/set_value_channel/main.nf:18:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      data // channel: [ file(infile) ]
      ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pacvar_pipeline/main.nf:116:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, bam, pbi, fail ->
                         ^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pacvar_pipeline/main.nf:155:9`: Variable was declared but not used

  ```nextflow
      def multiqc_reports = multiqc_report.toList()
          ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nextflow_pipeline/main.nf:43:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:20:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      valid_config = valid_config
      ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:72:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/pacvar.nf:102:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      pbmm2_input_filter_ch = pbmm2_input_ch.filter { meta, bam ->
                                                            ^^^
  ```

- Warning: `workflows/pacvar.nf:129:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, bams -> bams.size() > 1 }
                        ^^^^
  ```

- Warning: `workflows/pacvar.nf:134:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, bams -> bams.size() == 1 }
                        ^^^^
  ```

- Warning: `workflows/pacvar.nf:148:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta_fasta, fasta_file, meta_fai, fai_file -> [meta_fasta, fasta_file, fai_file] }
                                         ^^^^^^^^
  ```

- Warning: `workflows/pacvar.nf:156:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ordered_bam_ch = bam_bai_ch.map { meta, bam, bai -> [meta, bam] }
                                                   ^^^
  ```

- Warning: `workflows/pacvar.nf:157:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ordered_bai_ch = bam_bai_ch.map { meta, bam, bai -> [meta, bai] }
                                              ^^^
  ```

- Warning: `workflows/pacvar.nf:205:75`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      ? orderd_bam_bai_vcf_tbi_snp.vcf_tbi.map { meta, vcf, tbi -> [ meta, vcf ] }
                                                                            ^^^
  ```

- Warning: `workflows/pacvar.nf:230:90`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  cnv_input_bam_bai_maf_ch = bam_bai_vcf_snp_ch.map { meta, bam, bai, vcf, tbi ->
                                                                                           ^^^
  ```

- Warning: `workflows/pacvar.nf:248:83`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_cnv_vcf = BAM_CNV_VARIANT_CALLING.out.vcf_indexed.map { meta, vcf, tbi -> [ meta, vcf ] }
                                                                                    ^^^
  ```

- Warning: `workflows/pacvar.nf:268:122`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  (sv_input_bam_ch, sv_input_bai_ch, sv_input_maf_ch) = bam_bai_vcf_snp_ch.multiMap { meta, bam, bai, vcf, tbi ->
                                                                                                                           ^^^
  ```

- Warning: `workflows/pacvar.nf:321:74`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      ? orderd_bam_bai_vcf_tbi_sv.vcf_tbi.map { meta, vcf, tbi -> [ meta, vcf ] }
                                                                           ^^^
  ```
