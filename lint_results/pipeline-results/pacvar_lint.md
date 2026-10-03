# Nextflow lint results

- Generated: 2026-10-03T00:23:37.516516555Z
- Nextflow version: 26.09.1-edge
- Summary: 25 warnings

## :warning: Warnings

- Warning: `modules/nf-core/gunzip/main.nf:43:9`: Variable was declared but not used

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

- Warning: `subworkflows/local/bam_sv_variant_calling/main.nf:64:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_discover_bam_bai.map { meta, discover_dir, bam, bai -> [meta, discover_dir] },
                                                            ^^^
  ```

- Warning: `subworkflows/local/bam_sv_variant_calling/main.nf:64:64`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_discover_bam_bai.map { meta, discover_dir, bam, bai -> [meta, discover_dir] },
                                                                 ^^^
  ```

- Warning: `subworkflows/local/bam_sv_variant_calling/main.nf:66:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_discover_bam_bai.map { meta, discover_dir, bam, bai -> [meta, bam, bai] },
                                              ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/repeat_characterization/main.nf:30:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta_fasta, fasta_file, meta_fai, fai_file -> [meta_fasta, fasta_file, fai_file] }
                                         ^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pacvar_pipeline/main.nf:117:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, bam, pbi, fail ->
                         ^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pacvar_pipeline/main.nf:156:9`: Variable was declared but not used

  ```nextflow
      def multiqc_reports = multiqc_report.toList()
          ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/pacvar.nf:100:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      pbmm2_input_filter_ch = pbmm2_input_ch.filter { meta, bam ->
                                                            ^^^
  ```

- Warning: `workflows/pacvar.nf:126:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, bams -> bams.size() > 1 }
                        ^^^^
  ```

- Warning: `workflows/pacvar.nf:131:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, bams -> bams.size() == 1 }
                        ^^^^
  ```

- Warning: `workflows/pacvar.nf:145:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta_fasta, fasta_file, meta_fai, fai_file -> [meta_fasta, fasta_file, fai_file] }
                                         ^^^^^^^^
  ```

- Warning: `workflows/pacvar.nf:153:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ordered_bam_ch = bam_bai_ch.map { meta, bam, bai -> [meta, bam] }
                                                   ^^^
  ```

- Warning: `workflows/pacvar.nf:154:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ordered_bai_ch = bam_bai_ch.map { meta, bam, bai -> [meta, bai] }
                                              ^^^
  ```

- Warning: `workflows/pacvar.nf:202:75`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      ? orderd_bam_bai_vcf_tbi_snp.vcf_tbi.map { meta, vcf, tbi -> [ meta, vcf ] }
                                                                            ^^^
  ```

- Warning: `workflows/pacvar.nf:227:90`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  cnv_input_bam_bai_maf_ch = bam_bai_vcf_snp_ch.map { meta, bam, bai, vcf, tbi ->
                                                                                           ^^^
  ```

- Warning: `workflows/pacvar.nf:245:83`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_cnv_vcf = BAM_CNV_VARIANT_CALLING.out.vcf_indexed.map { meta, vcf, tbi -> [ meta, vcf ] }
                                                                                    ^^^
  ```

- Warning: `workflows/pacvar.nf:265:122`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  (sv_input_bam_ch, sv_input_bai_ch, sv_input_maf_ch) = bam_bai_vcf_snp_ch.multiMap { meta, bam, bai, vcf, tbi ->
                                                                                                                           ^^^
  ```

- Warning: `workflows/pacvar.nf:318:74`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      ? orderd_bam_bai_vcf_tbi_sv.vcf_tbi.map { meta, vcf, tbi -> [ meta, vcf ] }
                                                                           ^^^
  ```
