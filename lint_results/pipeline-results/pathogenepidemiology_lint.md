# Nextflow lint results

- Generated: 2026-07-30T00:29:50.106005950Z
- Nextflow version: 26.07.0-edge
- Summary: 23 warnings

## :warning: Warnings

- Warning: `workflows/download_references.nf:14:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_refs = Channel.of(params.queryurl, params.hosturl)
                ^^^^^^^
  ```

- Warning: `workflows/original_local.nf:45:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
    ch_samples = Channel
                 ^^^^^^^
  ```

- Warning: `workflows/original_local.nf:60:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
    ch_reads = ch_samples.map { meta, reads, platform ->
                                             ^^^^^^^^
  ```

- Warning: `workflows/original_local.nf:78:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
    ch_adapters = Channel.fromPath("${workflow.launchDir}/assets/adapters.fa")
                  ^^^^^^^
  ```

- Warning: `workflows/original_local.nf:86:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .join(ch_samples.map { meta, reads, platform -> tuple(meta, platform) }, by: 0)
                                   ^^^^^
  ```

- Warning: `workflows/original_local.nf:87:15`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .filter { meta, reads, platform ->
                ^^^^
  ```

- Warning: `workflows/original_local.nf:87:21`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .filter { meta, reads, platform ->
                      ^^^^^
  ```

- Warning: `workflows/original_local.nf:90:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .map { meta, reads, platform ->
                          ^^^^^^^^
  ```

- Warning: `workflows/original_local.nf:96:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .join(ch_samples.map { meta, reads, platform -> tuple(meta, platform) }, by: 0)
                                   ^^^^^
  ```

- Warning: `workflows/original_local.nf:97:15`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .filter { meta, reads, platform ->
                ^^^^
  ```

- Warning: `workflows/original_local.nf:97:21`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .filter { meta, reads, platform ->
                      ^^^^^
  ```

- Warning: `workflows/original_local.nf:100:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .map { meta, reads, platform ->
                          ^^^^^^^^
  ```

- Warning: `workflows/original_local.nf:117:3`: Variable was declared but not used

  ```nextflow
    varcalls_l = CLAIR3_CUSTOM(
    ^^^^^^^^^^
  ```

- Warning: `workflows/original_local.nf:141:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                            .map { meta, ref, fai_meta, fai -> tuple(meta, ref, fai) }
                                              ^^^^^^^^
  ```

- Warning: `workflows/original_local.nf:161:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
    ch_multiqc_input = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `workflows/original_local.nf:163:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          fastqc_out.zip.collect { meta, files -> files },
                                   ^^^^
  ```

- Warning: `workflows/original_local.nf:164:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          hostrm_prepped.stats.collect { meta, files -> files },
                                         ^^^^
  ```

- Warning: `workflows/original_local.nf:165:38`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          hostrm_prepped.log.collect { meta, files -> files },
                                       ^^^^
  ```

- Warning: `workflows/original_local.nf:166:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          hostrm_prepped.discarded.collect { meta, files -> files },
                                             ^^^^
  ```

- Warning: `workflows/original_local.nf:167:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          mm2stats.stats.collect { meta, files -> files },
                                   ^^^^
  ```

- Warning: `workflows/original_local.nf:168:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          bm3stats.stats.collect { meta, files -> files }
                                   ^^^^
  ```

- Warning: `workflows/prepare_references.nf:18:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_queryref = Channel.of(queryurl)
                    ^^^^^^^
  ```

- Warning: `workflows/prepare_references.nf:19:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_hostref  = Channel.of(hosturl)
                    ^^^^^^^
  ```
