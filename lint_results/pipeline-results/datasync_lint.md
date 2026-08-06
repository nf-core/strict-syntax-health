# Nextflow lint results

- Generated: 2026-08-06T00:25:54.313417690Z
- Nextflow version: 26.07.0-edge
- Summary: 7 warnings

## :warning: Warnings

- Warning: `subworkflows/local/utils_nfcore_datasync_pipeline/main.nf:195:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .findAll { it.trim() }
                     ^^
  ```

- Warning: `workflows/datasync.nf:103:26`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, checksum, hash, source -> [ meta.subMap(meta.keySet() - 'check_format'), 1 ] }
                           ^^^^^^^^
  ```

- Warning: `workflows/datasync.nf:103:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, checksum, hash, source -> [ meta.subMap(meta.keySet() - 'check_format'), 1 ] }
                                     ^^^^
  ```

- Warning: `workflows/datasync.nf:103:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, checksum, hash, source -> [ meta.subMap(meta.keySet() - 'check_format'), 1 ] }
                                           ^^^^^^
  ```

- Warning: `workflows/datasync.nf:115:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .collect { it.readLines() }
                                 ^^
  ```

- Warning: `workflows/datasync.nf:141:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, input, output, log -> [ meta, input, output ] }
                                      ^^^
  ```

- Warning: `workflows/datasync.nf:195:45`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(Channel.fromPath(params.input).collectFile(name: 'samplesheet.csv'))
                                              ^^^^^^^
  ```
