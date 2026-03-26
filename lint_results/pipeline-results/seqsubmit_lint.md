# Nextflow lint results

- Generated: 2026-03-26T00:27:13.906570146Z
- Nextflow version: 26.03.0-edge
- Summary: 1 error, 16 warnings

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

- Warning: `workflows/genomesubmit.nf:33:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      mags_or_bins_flag
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:79:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, fasta ->
                          ^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:85:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      genome_reads.filter { meta, reads -> meta.genome_coverage == null }
                                  ^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:110:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, fasta ->
                          ^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:133:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, fasta ->
                          ^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:164:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, fasta ->
                          ^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:266:26`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          genome_fasta.map{meta, fasta -> fasta}.collect(),
                           ^^^^
  ```

- Warning: `workflows/genomesubmit.nf:299:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_config        = channel.fromPath(
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:301:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_custom_config = params.multiqc_config ?
      ^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:304:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_logo          = params.multiqc_logo ?
      ^^^^^^^^^^^^^^^
  ```
