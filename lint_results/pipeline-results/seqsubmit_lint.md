# Nextflow lint results

- Generated: 2026-03-12T00:19:07.085143456Z
- Nextflow version: 26.02.0-edge
- Summary: 1 error, 12 warnings

## :x: Errors

- Error: `subworkflows/local/rna_detection.nf:29:24`: `fasta` is already declared

  ```nextflow
          fasta.map {id, fasta -> [id, fasta, "bac"]}
                         ^^^^^
  ```

## :warning: Warnings

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

- Warning: `modules/local/registerstudy/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/registerstudy/main.nf:46:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/barrnap/main.nf:45:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/rna_detection.nf:27:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:27:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      mags_or_bins_flag
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:60:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      genome_fasta.filter { meta, fasta -> meta.RNA_presence == null }
                                  ^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:63:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      genome_fasta.filter { meta, fasta -> meta.RNA_presence != null }
                                  ^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:86:17`: Variable was declared but not used

  ```nextflow
              def row = [
                  ^^^
  ```

- Warning: `workflows/genomesubmit.nf:113:26`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          genome_fasta.map{meta, fasta -> fasta}.collect(),
                           ^^^^
  ```
