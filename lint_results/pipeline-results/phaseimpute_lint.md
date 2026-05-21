# Nextflow lint results

- Generated: 2026-05-21T00:42:05.203109943Z
- Nextflow version: 26.04.1
- Summary: 4 warnings

## :warning: Warnings

- Warning: `subworkflows/local/prepare_genome/main.nf:42:5`: Variable was declared but not used

  ```nextflow
      ch_fasta_fai_gzi = ch_fasta
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phaseimpute_pipeline/main.nf:423:5`: Variable was declared but not used

  ```nextflow
      ch_fasta_index = ch_ref_gen.map{ meta, fasta, fai, gzi -> [
      ^^^^^^^^^^^^^^
  ```

- Warning: `workflows/phaseimpute/main.nf:131:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, map_file ->
                    ^^^^
  ```

- Warning: `workflows/phaseimpute/main.nf:311:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          if (params.tools.split(',').any{ it in ["stitch", "quilt"] }) {
                                           ^^
  ```
