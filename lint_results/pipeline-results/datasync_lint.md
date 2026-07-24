# Nextflow lint results

- Generated: 2026-07-24T00:26:53.920427862Z
- Nextflow version: 26.07.0-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `subworkflows/local/utils_nfcore_datasync_pipeline/main.nf:195:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .findAll { it.trim() }
                     ^^
  ```

- Warning: `workflows/datasync.nf:102:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, input, output, log -> [ meta, input, output ]}
                                      ^^^
  ```

- Warning: `workflows/datasync.nf:153:45`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(Channel.fromPath(params.input).collectFile(name: 'samplesheet.csv'))
                                              ^^^^^^^
  ```
