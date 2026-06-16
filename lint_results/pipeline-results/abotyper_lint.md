# Nextflow lint results

- Generated: 2026-06-16T20:15:25.974556555Z
- Nextflow version: 26.04.3
- Summary: 65 warnings

## :warning: Warnings

- Warning: `main.nf:46:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      exon6fai = params.exon6fai ? Channel.fromPath(params.exon6fai).map { it -> [[id: it.baseName, exon: 'exon6'], it] } : Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `main.nf:46:123`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      exon6fai = params.exon6fai ? Channel.fromPath(params.exon6fai).map { it -> [[id: it.baseName, exon: 'exon6'], it] } : Channel.empty()
                                                                                                                            ^^^^^^^
  ```

- Warning: `main.nf:47:38`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      exon6fasta = params.exon6fasta ? Channel.fromPath(params.exon6fasta).map { it -> [[id: it.baseName, exon: 'exon6'], it] } : Channel.empty()
                                       ^^^^^^^
  ```

- Warning: `main.nf:47:129`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      exon6fasta = params.exon6fasta ? Channel.fromPath(params.exon6fasta).map { it -> [[id: it.baseName, exon: 'exon6'], it] } : Channel.empty()
                                                                                                                                  ^^^^^^^
  ```

- Warning: `main.nf:48:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      exon7fai = params.exon7fai ? Channel.fromPath(params.exon7fai).map { it -> [[id: it.baseName, exon: 'exon7'], it] } : Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `main.nf:48:123`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      exon7fai = params.exon7fai ? Channel.fromPath(params.exon7fai).map { it -> [[id: it.baseName, exon: 'exon7'], it] } : Channel.empty()
                                                                                                                            ^^^^^^^
  ```

- Warning: `main.nf:49:38`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      exon7fasta = params.exon7fasta ? Channel.fromPath(params.exon7fasta).map { it -> [[id: it.baseName, exon: 'exon7'], it] } : Channel.empty()
                                       ^^^^^^^
  ```

- Warning: `main.nf:49:129`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      exon7fasta = params.exon7fasta ? Channel.fromPath(params.exon7fasta).map { it -> [[id: it.baseName, exon: 'exon7'], it] } : Channel.empty()
                                                                                                                                  ^^^^^^^
  ```

- Warning: `main.nf:50:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      logo = params.logo ? Channel.fromPath(params.logo).collect() : Channel.empty()
                           ^^^^^^^
  ```

- Warning: `main.nf:50:68`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      logo = params.logo ? Channel.fromPath(params.logo).collect() : Channel.empty()
                                                                     ^^^^^^^
  ```

- Warning: `main.nf:62:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = ABOTYPER.out.multiqc_report
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/abo/getabosnps/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/mpileupstats/main.nf:32:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:26:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { sample_meta, fastq, ref_meta, fasta ->
                                 ^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:26:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { sample_meta, fastq, ref_meta, fasta ->
                                                  ^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:38:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_minimap_ready.map { meta, fastq, fasta -> [meta, fastq] },
                                              ^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:39:38`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_minimap_ready.map { meta, fastq, fasta -> [meta, fasta] },
                                       ^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:55:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                              ^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:55:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                                   ^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:55:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                                                    ^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:55:68`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                                                                     ^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:60:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_coverage_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                                                      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:60:65`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_coverage_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                                                                  ^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:60:72`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_coverage_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                                                                         ^^^^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:60:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_coverage_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                                                                                   ^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:63:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_coverage_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                                  ^^^^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:63:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_coverage_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                                            ^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:63:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_coverage_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                                                 ^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:63:72`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_coverage_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                                                                         ^^^^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:81:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                              ^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:81:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                                   ^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:81:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                                                    ^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:81:68`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                                                                     ^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:86:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_stats_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                                                   ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:86:62`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_stats_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                                                               ^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:86:69`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_stats_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                                                                      ^^^^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:86:79`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_stats_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                                                                                ^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:89:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_stats_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                               ^^^^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:89:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_stats_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                                         ^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:89:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_stats_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                                              ^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:89:69`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_stats_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                                                                      ^^^^^^^^
  ```

- Warning: `subworkflows/local/predictabophenotype/main.nf:50:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def exon_dir = sample_dir.resolve(it.exon)
                                                    ^^
  ```

- Warning: `subworkflows/local/predictabophenotype/main.nf:52:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it.file.copyTo(exon_dir.resolve(it.file.name))
                  ^^
  ```

- Warning: `subworkflows/local/predictabophenotype/main.nf:52:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it.file.copyTo(exon_dir.resolve(it.file.name))
                                                  ^^
  ```

- Warning: `subworkflows/local/predictabophenotype/main.nf:70:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      abo_results = ABO_SNPS2PHENO.out.txt
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_haploscan/main.nf:21:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_bed   // channel: [ val(meta1), path(bed)   ]  — accepted but not used
      ^^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_haploscan/main.nf:31:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { fasta_meta, fasta, fai_meta, fai ->
                                ^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_haploscan/main.nf:31:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { fasta_meta, fasta, fai_meta, fai ->
                                                 ^^^
  ```

- Warning: `subworkflows/local/variant_calling_haploscan/main.nf:35:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { fasta_meta, fasta, fai_meta, fai ->
                                    ^^^^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_haploscan/main.nf:42:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, fasta_meta, fasta, fai ->
                              ^^^
  ```

- Warning: `subworkflows/local/variant_calling_haploscan/main.nf:42:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, fasta_meta, fasta, fai ->
                                   ^^^
  ```

- Warning: `subworkflows/local/variant_calling_haploscan/main.nf:42:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, fasta_meta, fasta, fai ->
                                                    ^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_haploscan/main.nf:42:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, fasta_meta, fasta, fai ->
                                                           ^^^
  ```

- Warning: `subworkflows/local/variant_calling_haploscan/main.nf:48:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_haploscan_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai ->
                                                       ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_haploscan/main.nf:48:66`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_haploscan_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai ->
                                                                   ^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_haploscan/main.nf:48:73`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_haploscan_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai ->
                                                                          ^^^
  ```

- Warning: `subworkflows/local/variant_calling_haploscan/main.nf:51:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_haploscan_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai ->
                                   ^^^^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_haploscan/main.nf:51:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_haploscan_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai ->
                                             ^^^
  ```

- Warning: `subworkflows/local/variant_calling_haploscan/main.nf:51:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_haploscan_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai ->
                                                  ^^^
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

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:76:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/abotyper.nf:37:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      logo // channel: png from params.logo (custom pathwest logo)
      ^^^^
  ```

- Warning: `workflows/abotyper.nf:73:68`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(FASTQC.out.zip.collect{it[1]})
                                                                     ^^
  ```

- Warning: `workflows/abotyper.nf:115:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```
