# Nextflow lint results

- Generated: 2026-09-16T00:18:20.234981455Z
- Nextflow version: 26.08.0-edge
- Summary: 19 warnings

## :warning: Warnings

- Warning: `main.nf:46:54`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      abo_reference_fai   = params.abo_reference_fai ? Channel.fromPath(params.abo_reference_fai)
                                                       ^^^^^^^
  ```

- Warning: `main.nf:47:50`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          .map { it -> [[id: it.baseName], it] } : Channel.empty()
                                                   ^^^^^^^
  ```

- Warning: `main.nf:48:56`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      abo_reference_fasta = params.abo_reference_fasta ? Channel.fromPath(params.abo_reference_fasta)
                                                         ^^^^^^^
  ```

- Warning: `main.nf:49:50`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          .map { it -> [[id: it.baseName], it] } : Channel.empty()
                                                   ^^^^^^^
  ```

- Warning: `main.nf:50:53`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      clair3_model_url    = params.clair3_model_url ? Channel.value(params.clair3_model_url) :
                                                      ^^^^^^^
  ```

- Warning: `main.nf:51:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.empty()
          ^^^^^^^
  ```

- Warning: `main.nf:52:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      logo = params.logo ? Channel.fromPath(params.logo).collect() : Channel.empty()
                           ^^^^^^^
  ```

- Warning: `main.nf:52:68`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      logo = params.logo ? Channel.fromPath(params.logo).collect() : Channel.empty()
                                                                     ^^^^^^^
  ```

- Warning: `main.nf:53:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      abo_panel = params.abo_panel ? Channel.fromPath(params.abo_panel).collect() : Channel.empty()
                                     ^^^^^^^
  ```

- Warning: `main.nf:53:83`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      abo_panel = params.abo_panel ? Channel.fromPath(params.abo_panel).collect() : Channel.empty()
                                                                                    ^^^^^^^
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

- Warning: `subworkflows/local/predictabophenotype/main.nf:50:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it.file.copyTo(combined_dir.resolve(it.file.name))
                  ^^
  ```

- Warning: `subworkflows/local/predictabophenotype/main.nf:50:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it.file.copyTo(combined_dir.resolve(it.file.name))
                                                      ^^
  ```

- Warning: `subworkflows/local/variants_quantification/main.nf:33:5`: Variable was declared but not used

  ```nextflow
      ch_fasta_fai = ch_fasta
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/variants_quantification/main.nf:35:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { fasta_meta, fasta, fai_meta, fai -> [fasta_meta, fasta, fai] }
                                    ^^^^^^^^
  ```

- Warning: `workflows/abotyper.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      logo                 // channel: png from params.logo (custom pathwest logo)
      ^^^^
  ```

- Warning: `workflows/abotyper.nf:49:68`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(FASTQC.out.zip.collect{it[1]})
                                                                     ^^
  ```

- Warning: `workflows/abotyper.nf:103:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```
