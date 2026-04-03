# Nextflow lint results

- Generated: 2026-04-03T00:25:00.865544300Z
- Nextflow version: 26.03.1-edge
- Summary: 77 warnings

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

- Warning: `subworkflows/local/predictabophenotype/main.nf:44:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def exon_dir = sample_dir.resolve(it.exon)
                                                    ^^
  ```

- Warning: `subworkflows/local/predictabophenotype/main.nf:46:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it.file.copyTo(exon_dir.resolve(it.file.name))
                  ^^
  ```

- Warning: `subworkflows/local/predictabophenotype/main.nf:46:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it.file.copyTo(exon_dir.resolve(it.file.name))
                                                  ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_abotyper_pipeline/main.nf:30:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_abotyper_pipeline/main.nf:33:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_abotyper_pipeline/main.nf:52:5`: Variable was declared but not used

  ```nextflow
      before_text = """
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_abotyper_pipeline/main.nf:62:5`: Variable was declared but not used

  ```nextflow
      after_text = """${workflow.manifest.doi ? "\n* The pipeline\n" : ""}${workflow.manifest.doi.tokenize(",").collect { doi -> "    https://doi.org/${doi.trim().replace('https://doi.org/','')}"}.join("\n")}${workflow.manifest.doi ? "\n" : ""}
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_abotyper_pipeline/main.nf:69:5`: Variable was declared but not used

  ```nextflow
      command = "nextflow run ${workflow.manifest.name} -profile <docker/singularity/.../institute> --input samplesheet.csv --outdir <OUTDIR>"
      ^^^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:33:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, bed_meta, bed ->
                              ^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:33:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, bed_meta, bed ->
                                   ^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:33:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, bed_meta, bed ->
                                                  ^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:36:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { bam_meta, bam, bai, bed_meta, bed ->
                                     ^^^^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:43:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { fasta_meta, fasta, fai_meta, fai ->
                                ^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:43:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { fasta_meta, fasta, fai_meta, fai ->
                                                 ^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:48:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { fasta_meta, fasta, fai_meta, fai ->
                                    ^^^^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:55:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, bed, fasta_meta, fasta, fai ->
                              ^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:55:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, bed, fasta_meta, fasta, fai ->
                                   ^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:55:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, bed, fasta_meta, fasta, fai ->
                                        ^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:55:56`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, bed, fasta_meta, fasta, fai ->
                                                         ^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:55:63`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, bed, fasta_meta, fasta, fai ->
                                                                ^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:66:57`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_fasta_matched.map { bam_meta, bam, bai, bed, fasta_meta, fasta, fai ->
                                                          ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:66:69`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_fasta_matched.map { bam_meta, bam, bai, bed, fasta_meta, fasta, fai ->
                                                                      ^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:66:76`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_fasta_matched.map { bam_meta, bam, bai, bed, fasta_meta, fasta, fai ->
                                                                             ^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:69:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_fasta_matched.map { bam_meta, bam, bai, bed, fasta_meta, fasta, fai ->
                                 ^^^^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:69:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_fasta_matched.map { bam_meta, bam, bai, bed, fasta_meta, fasta, fai ->
                                           ^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:69:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_fasta_matched.map { bam_meta, bam, bai, bed, fasta_meta, fasta, fai ->
                                                ^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:69:52`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_fasta_matched.map { bam_meta, bam, bai, bed, fasta_meta, fasta, fai ->
                                                     ^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:77:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { mpileup_meta, mpileup, fasta_meta, fasta ->
                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:77:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { mpileup_meta, mpileup, fasta_meta, fasta ->
                                                       ^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:85:57`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_nucl_freq_input.map { mpileup_meta, mpileup, fasta_meta, fasta ->
                                                          ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:85:69`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_nucl_freq_input.map { mpileup_meta, mpileup, fasta_meta, fasta ->
                                                                      ^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:88:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_nucl_freq_input.map { mpileup_meta, mpileup, fasta_meta, fasta ->
                                   ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:88:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_nucl_freq_input.map { mpileup_meta, mpileup, fasta_meta, fasta ->
                                                 ^^^^^^^
  ```

- Warning: `workflows/abotyper.nf:36:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      logo // channel: png from params.logo (custom pathwest logo)
      ^^^^
  ```

- Warning: `workflows/abotyper.nf:149:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .mix(FASTQC.out.zip.map { meta, files -> files }.flatten())
                                    ^^^^
  ```

- Warning: `workflows/abotyper.nf:150:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .mix(MINIMAP2_ALIGN_READS.out.coverage.map { meta, cov -> cov })
                                                       ^^^^
  ```

- Warning: `workflows/abotyper.nf:151:56`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .mix(VARIANTS_QUANTIFICATION.out.metrics.map { meta, metrics -> metrics })
                                                         ^^^^
  ```
