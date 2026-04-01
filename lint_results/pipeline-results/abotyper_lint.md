# Nextflow lint results

- Generated: 2026-04-01T00:27:06.016580130Z
- Nextflow version: 26.03.1-edge
- Summary: 6 errors, 64 warnings

## :x: Errors

- Error: `nextflow.config:314:32`: `manifest` is not defined

  ```nextflow
  \033[0;35m  nf-core/abotyper ${manifest.version}\033[0m
                                 ^^^^^^^^
  ```

- Error: `nextflow.config:317:26`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                           ^^^^^^^^
  ```

- Error: `nextflow.config:317:69`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                      ^^^^^^^^
  ```

- Error: `nextflow.config:317:186`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                                                                                                                                           ^^^^^^^^
  ```

- Error: `nextflow.config:326:22`: `validation` is not defined

  ```nextflow
          beforeText = validation.help.beforeText
                       ^^^^^^^^^^
  ```

- Error: `nextflow.config:327:21`: `validation` is not defined

  ```nextflow
          afterText = validation.help.afterText
                      ^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `modules/local/abo/getabosnps/main.nf:19:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/mpileupstats/main.nf:31:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/minimap2/align/main.nf:67:9`: Variable was declared but not used

  ```nextflow
      def target = reference ?: (bam_input ? error("BAM input requires reference") : reads)
          ^^^^^^
  ```

- Warning: `nextflow.config:317:129`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                                                                                  ^^
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

- Warning: `subworkflows/local/minimap_align_exons/main.nf:56:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                              ^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:56:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                                   ^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:56:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                                                    ^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:56:68`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai ->
                                                                     ^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:61:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_coverage_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai -> [bam_meta, bam, bai] },
                                                      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:61:65`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_coverage_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai -> [bam_meta, bam, bai] },
                                                                  ^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:61:72`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_coverage_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai -> [bam_meta, bam, bai] },
                                                                         ^^^^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:61:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_coverage_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai -> [bam_meta, bam, bai] },
                                                                                   ^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:62:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_coverage_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai -> [fasta_meta, fasta] },
                                  ^^^^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:62:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_coverage_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai -> [fasta_meta, fasta] },
                                            ^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:62:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_coverage_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai -> [fasta_meta, fasta] },
                                                 ^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:62:72`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_coverage_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai -> [fasta_meta, fasta] },
                                                                         ^^^^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:62:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_coverage_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai -> [fasta_meta, fasta] },
                                                                                   ^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:63:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_coverage_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai -> [fai_meta, fai] },
                                  ^^^^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:63:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_coverage_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai -> [fai_meta, fai] },
                                            ^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:63:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_coverage_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai -> [fai_meta, fai] },
                                                 ^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:63:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_coverage_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai -> [fai_meta, fai] },
                                                      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:63:65`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_coverage_input.map { bam_meta, bam, bai, fasta_meta, fasta, fai_meta, fai -> [fai_meta, fai] },
                                                                  ^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:80:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, fasta_meta, fasta ->
                              ^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:80:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, fasta_meta, fasta ->
                                   ^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:80:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bai, fasta_meta, fasta ->
                                                    ^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:85:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_stats_input.map { bam_meta, bam, bai, fasta_meta, fasta -> [bam_meta, bam, bai] },
                                                   ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:85:62`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_stats_input.map { bam_meta, bam, bai, fasta_meta, fasta -> [bam_meta, bam, bai] },
                                                               ^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:86:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_stats_input.map { bam_meta, bam, bai, fasta_meta, fasta -> [fasta_meta, fasta] },
                               ^^^^^^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:86:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_stats_input.map { bam_meta, bam, bai, fasta_meta, fasta -> [fasta_meta, fasta] },
                                         ^^^
  ```

- Warning: `subworkflows/local/minimap_align_exons/main.nf:86:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_stats_input.map { bam_meta, bam, bai, fasta_meta, fasta -> [fasta_meta, fasta] },
                                              ^^^
  ```

- Warning: `subworkflows/local/predictabophenotype/main.nf:45:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def exon_dir = sample_dir.resolve(it.exon)
                                                    ^^
  ```

- Warning: `subworkflows/local/predictabophenotype/main.nf:47:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it.file.copyTo(exon_dir.resolve(it.file.name))
                  ^^
  ```

- Warning: `subworkflows/local/predictabophenotype/main.nf:47:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

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

- Warning: `subworkflows/local/utils_nfcore_abotyper_pipeline/main.nf:74:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:7:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_bai // channel: [ val(meta), path(bai)]    - BAI file from minimap2 alignment
      ^^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:9:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fai // channel: [ val(meta1), path(fai)]   - fasta index for the references
      ^^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:19:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bed_meta, bed ->
                              ^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:19:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bed_meta, bed ->
                                             ^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:22:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { bam_meta, bam, bed_meta, bed ->
                                ^^^^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:29:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bed, fasta_meta, fasta ->
                              ^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:29:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bed, fasta_meta, fasta ->
                                   ^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:29:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { bam_meta, bam, bed, fasta_meta, fasta ->
                                                    ^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:40:52`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_fasta_matched.map { bam_meta, bam, bed, fasta_meta, fasta -> [bam_meta, bam, bed] },
                                                     ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:40:64`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_fasta_matched.map { bam_meta, bam, bed, fasta_meta, fasta -> [bam_meta, bam, bed] },
                                                                 ^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:41:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_fasta_matched.map { bam_meta, bam, bed, fasta_meta, fasta -> [fasta_meta, fasta] },
                                 ^^^^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:41:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_fasta_matched.map { bam_meta, bam, bed, fasta_meta, fasta -> [fasta_meta, fasta] },
                                           ^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:41:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_fasta_matched.map { bam_meta, bam, bed, fasta_meta, fasta -> [fasta_meta, fasta] },
                                                ^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:49:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { mpileup_meta, mpileup, fasta_meta, fasta ->
                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:49:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { mpileup_meta, mpileup, fasta_meta, fasta ->
                                                       ^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:57:57`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_nucl_freq_input.map { mpileup_meta, mpileup, fasta_meta, fasta -> [mpileup_meta, mpileup] },
                                                          ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:57:69`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_nucl_freq_input.map { mpileup_meta, mpileup, fasta_meta, fasta -> [mpileup_meta, mpileup] },
                                                                      ^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:58:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_nucl_freq_input.map { mpileup_meta, mpileup, fasta_meta, fasta -> [fasta_meta, fasta] },
                                   ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/variant_calling_mpileup/main.nf:58:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_nucl_freq_input.map { mpileup_meta, mpileup, fasta_meta, fasta -> [fasta_meta, fasta] },
                                                 ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:101:98`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      return ch_versions.unique().map { version -> processVersionsFromYAML(version) }.unique().mix(Channel.of(workflowVersionToYAML()))
                                                                                                   ^^^^^^^
  ```

- Warning: `workflows/abotyper.nf:36:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      logo // channel: png from params.logo (custom pathwest logo)
      ^^^^
  ```

- Warning: `workflows/abotyper.nf:134:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .mix(FASTQC.out.zip.map { meta, files -> files }.flatten())
                                    ^^^^
  ```

- Warning: `workflows/abotyper.nf:135:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .mix(MINIMAP2_ALIGN_READS.out.coverage.map { meta, cov -> cov })
                                                       ^^^^
  ```

- Warning: `workflows/abotyper.nf:136:56`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .mix(VARIANTS_QUANTIFICATION.out.metrics.map { meta, metrics -> metrics })
                                                         ^^^^
  ```
