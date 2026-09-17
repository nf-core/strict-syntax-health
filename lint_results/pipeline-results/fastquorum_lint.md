# Nextflow lint results

- Generated: 2026-09-17T00:18:53.554603539Z
- Nextflow version: 26.08.0-edge
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
