# Nextflow lint results

- Generated: 2026-03-31T00:29:22.458385672Z
- Nextflow version: 26.03.1-edge
- Summary: 1 error, 14 warnings

## :x: Errors

- Error: `subworkflows/local/rna_detection.nf:29:24`: `fasta` is already declared

  ```nextflow
          fasta.map {id, fasta -> [id, fasta, "bac"]}
                         ^^^^^
  ```

## :warning: Warnings

- Warning: `conf/modules.config:59:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  saveAs: { filename -> "db" }
                            ^^^^^^^^
  ```

- Warning: `conf/modules.config:65:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  saveAs: { filename -> "tax" }
                            ^^^^^^^^
  ```

- Warning: `modules/local/generate_assembly_manifest/main.nf:20:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/generate_assembly_manifest/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/generate_assembly_manifest/main.nf:39:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/barrnap/main.nf:45:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/genome_evaluation.nf:26:5`: Variable was declared but not used

  ```nextflow
      ch_versions = channel.empty()
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fasta_classify_catpack/main.nf:39:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, db ->
                    ^^^^
  ```

- Warning: `workflows/genomesubmit.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      mags_or_bins_flag
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:125:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, fasta ->
                          ^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:148:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, fasta ->
                          ^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:179:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, fasta ->
                          ^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:284:38`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          fasta_updated_with_stats.map{meta, fasta -> fasta}.collect(),
                                       ^^^^
  ```

- Warning: `workflows/genomesubmit.nf:306:12`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .map { id, full_meta, fasta, manifest ->
             ^^
  ```
