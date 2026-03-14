# Nextflow lint results

- Generated: 2026-03-14T00:22:56.545502782Z
- Nextflow version: 26.02.0-edge
- Summary: 1 error, 21 warnings

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

- Warning: `subworkflows/local/genome_evaluation.nf:26:5`: Variable was declared but not used

  ```nextflow
      ch_versions = channel.empty()
      ^^^^^^^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:30:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      mags_or_bins_flag
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:76:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      genome_reads.filter { meta, reads -> meta.genome_coverage == null }
                                  ^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:79:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      genome_fasta.filter { meta, fasta -> meta.genome_coverage == null }
                                  ^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:82:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      genome_fasta.filter { meta, fasta -> meta.genome_coverage != null }
                                  ^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:106:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      fasta_updated_with_coverage.filter { meta, fasta -> meta.RNA_presence == null }
                                                 ^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:109:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      fasta_updated_with_coverage.filter { meta, fasta -> meta.RNA_presence != null }
                                                 ^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:130:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      fasta_updated_with_rna.filter { meta, fasta -> meta.completeness == null || meta.contamination == null || meta.stats_generation_software == null }
                                            ^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:133:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      fasta_updated_with_rna.filter { meta, fasta -> meta.completeness != null && meta.contamination != null && meta.stats_generation_software != null}
                                            ^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:143:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { process_name, tool_name, version_output -> return "${tool_name}_v${version_output}"
                 ^^^^^^^^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:161:5`: Variable was declared but not used

  ```nextflow
      genome_metadata_csv = fasta_updated_with_stats
      ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:163:17`: Variable was declared but not used

  ```nextflow
              def row = [
                  ^^^
  ```

- Warning: `workflows/genomesubmit.nf:222:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_config        = channel.fromPath(
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:224:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_custom_config = params.multiqc_config ?
      ^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:227:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_logo          = params.multiqc_logo ?
      ^^^^^^^^^^^^^^^
  ```
