# Nextflow lint results

- Generated: 2026-07-29T00:27:32.151490132Z
- Nextflow version: 26.07.0-edge
- Summary: 5 warnings

## :warning: Warnings

- Warning: `subworkflows/local/utils_nfcore_fastquorum_pipeline/main.nf:30:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_fastquorum_pipeline/main.nf:33:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `workflows/fastquorum.nf:63:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, bam ->
                          ^^^
  ```

- Warning: `workflows/fastquorum.nf:70:41`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fastqtobam.correct.first().map { meta, bam ->
                                          ^^^^
  ```

- Warning: `workflows/fastquorum.nf:70:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fastqtobam.correct.first().map { meta, bam ->
                                                ^^^
  ```
