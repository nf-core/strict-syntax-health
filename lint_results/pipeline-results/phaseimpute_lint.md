# Nextflow lint results

- Generated: 2026-05-20T00:43:35.140455187Z
- Nextflow version: 26.04.1
- Summary: 5 warnings

## :warning: Warnings

- Warning: `subworkflows/local/prepare_genome/main.nf:42:5`: Variable was declared but not used

  ```nextflow
      ch_fasta_fai_gzi = ch_fasta
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phaseimpute_pipeline/main.nf:417:5`: Variable was declared but not used

  ```nextflow
      ch_fasta_index = ch_ref_gen.map{ meta, fasta, fai, gzi -> [
      ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
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
