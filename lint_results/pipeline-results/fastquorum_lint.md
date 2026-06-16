# Nextflow lint results

- Generated: 2026-06-16T20:24:08.886678908Z
- Nextflow version: 26.04.3
- Summary: 10 warnings

## :warning: Warnings

- Warning: `main.nf:152:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = FASTQUORUM.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:20:5`: Variable was declared but not used

  ```nextflow
      versions = channel.empty()
      ^^^^^^^^
  ```

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

- Warning: `subworkflows/nf-core/utils_nextflow_pipeline/main.nf:43:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:20:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      valid_config = valid_config
      ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:76:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/fastquorum.nf:65:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, bam ->
                          ^^^
  ```

- Warning: `workflows/fastquorum.nf:72:41`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fastqtobam.correct.first().map { meta, bam ->
                                          ^^^^
  ```

- Warning: `workflows/fastquorum.nf:72:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fastqtobam.correct.first().map { meta, bam ->
                                                ^^^
  ```
