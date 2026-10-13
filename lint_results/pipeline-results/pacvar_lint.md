# Nextflow lint results

- Generated: 2026-10-13T00:27:04.851078327Z
- Nextflow version: 26.10.0
- Summary: 50 warnings

## :warning: Warnings

- Warning: `modules/nf-core/bcftools/index/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bcftools/sort/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/deepvariant/callvariants/main.nf:16:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/deepvariant/makeexamples/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/deepvariant/postprocessvariants/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/deepvariant/rundeepvariant/main.nf:26:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/ensemblvep/download/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/ensemblvep/vep/main.nf:29:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/fastqc/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/fibertoolsrs/addnucleosomes/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/fibertoolsrs/extract/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/fibertoolsrs/predictm6a/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gatk4/haplotypecaller/main.nf:24:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gunzip/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gunzip/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/hificnv/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/hiphase/main.nf:37:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/lima/main.nf:31:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/multiqc/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/pbcpgtools/alignedbamtocpgscores/main.nf:25:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/pbmm2/align/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/pbsv/call/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/pbsv/call/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/pbsv/discover/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/pbsv/discover/main.nf:36:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/pbtk/pbmerge/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/pbtk/pbmerge/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/samtools/index/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/sort/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/sawfish/discover/main.nf:39:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/sawfish/jointcall/main.nf:29:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/tabix/bgzip/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/trgt/genotype/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/trgt/genotype/main.nf:45:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/trgt/plot/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
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

- Warning: `workflows/pacvar.nf:97:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      pbmm2_input_filter_ch = pbmm2_input_ch.filter { meta, bam ->
                                                            ^^^
  ```

- Warning: `workflows/pacvar.nf:123:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, bams -> bams.size() > 1 }
                        ^^^^
  ```

- Warning: `workflows/pacvar.nf:128:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, bams -> bams.size() == 1 }
                        ^^^^
  ```

- Warning: `workflows/pacvar.nf:142:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta_fasta, fasta_file, meta_fai, fai_file -> [meta_fasta, fasta_file, fai_file] }
                                         ^^^^^^^^
  ```

- Warning: `workflows/pacvar.nf:150:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ordered_bam_ch = bam_bai_ch.map { meta, bam, bai -> [meta, bam] }
                                                   ^^^
  ```

- Warning: `workflows/pacvar.nf:151:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ordered_bai_ch = bam_bai_ch.map { meta, bam, bai -> [meta, bai] }
                                              ^^^
  ```
