# Nextflow lint results

- Generated: 2026-11-14T00:11:45.643022587Z
- Nextflow version: 26.10.6
- Summary: 31 warnings

## :warning: Warnings

- Warning: `main.nf:45:54`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      abo_reference_fai   = params.abo_reference_fai ? Channel.fromPath(params.abo_reference_fai)
                                                       ^^^^^^^
  ```

- Warning: `main.nf:46:50`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          .map { it -> [[id: it.baseName], it] } : Channel.empty()
                                                   ^^^^^^^
  ```

- Warning: `main.nf:47:56`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      abo_reference_fasta = params.abo_reference_fasta ? Channel.fromPath(params.abo_reference_fasta)
                                                         ^^^^^^^
  ```

- Warning: `main.nf:48:50`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          .map { it -> [[id: it.baseName], it] } : Channel.empty()
                                                   ^^^^^^^
  ```

- Warning: `main.nf:59:63`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          path:     (!clair3_url && params.clair3_model_path) ? Channel.fromPath(params.clair3_model_path, type: 'dir', checkIfExists: true).first() : null,
                                                                ^^^^^^^
  ```

- Warning: `main.nf:63:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      abo_panel = params.abo_panel ? Channel.fromPath(params.abo_panel, checkIfExists: true).collect() : Channel.value([])
                                     ^^^^^^^
  ```

- Warning: `main.nf:63:104`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      abo_panel = params.abo_panel ? Channel.fromPath(params.abo_panel, checkIfExists: true).collect() : Channel.value([])
                                                                                                         ^^^^^^^
  ```

- Warning: `main.nf:66:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ? Channel.fromPath(params.abo_clair3_region_bed, checkIfExists: true).collect()
            ^^^^^^^
  ```

- Warning: `main.nf:67:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.value([])
            ^^^^^^^
  ```

- Warning: `modules/local/abo/evidence/main.nf:42:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/clair3/downloadmodel/main.nf:24:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bcftools/norm/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bcftools/query/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bcftools/view/main.nf:24:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/clair3/main.nf:29:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/minimap2/align/main.nf:28:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/multiqc/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/nanoplot/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/coverage/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/flagstat/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/mpileup/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/stats/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `subworkflows/local/minimap2_align_reads/main.nf:30:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta_fa, fa, meta_fai, fai -> [ [id: 'ABO_REF'], fa, fai ] }
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/minimap2_align_reads/main.nf:30:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta_fa, fa, meta_fai, fai -> [ [id: 'ABO_REF'], fa, fai ] }
                              ^^^^^^^^
  ```

- Warning: `subworkflows/local/variants_quantification/main.nf:39:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { fasta_meta, fasta, fai_meta, fai -> [fasta_meta, fasta, fai] }
                                    ^^^^^^^^
  ```

- Warning: `subworkflows/local/variants_quantification/main.nf:75:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it[3] == null }
                    ^^
  ```

- Warning: `subworkflows/local/variants_quantification/main.nf:76:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .subscribe { log.warn "Clair3 produced no gVCF for sample '${it[0].id}': relying on the BAM pileup alone (flagged REVIEW)" }
                                                                       ^^
  ```

- Warning: `workflows/abotyper.nf:49:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(NANOPLOT.out.txt.collect{it[1]})
                                                                       ^^
  ```

- Warning: `workflows/abotyper.nf:60:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          MINIMAP2_ALIGN_READS.out.stats.collect{ it[1] },
                                                  ^^
  ```

- Warning: `workflows/abotyper.nf:61:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          MINIMAP2_ALIGN_READS.out.flagstat.collect{ it[1] },
                                                     ^^
  ```

- Warning: `workflows/abotyper.nf:116:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```
