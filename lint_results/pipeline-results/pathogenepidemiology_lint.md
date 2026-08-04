# Nextflow lint results

- Generated: 2026-08-04T00:32:49.440760936Z
- Nextflow version: 26.07.0-edge
- Summary: 23 warnings

## :warning: Warnings

- Warning: `workflows/download_references.nf:14:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_refs = Channel.of(params.queryurl, params.hosturl)
                ^^^^^^^
  ```

- Warning: `workflows/original_local.nf:65:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .join(ch_samples.map { meta, reads, platform -> tuple(meta, platform) }, by: 0)
                                   ^^^^^
  ```

- Warning: `workflows/original_local.nf:66:15`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .filter { meta, reads, platform ->
                ^^^^
  ```

- Warning: `workflows/original_local.nf:66:21`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .filter { meta, reads, platform ->
                      ^^^^^
  ```

- Warning: `workflows/original_local.nf:69:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .map { meta, reads, platform ->
                          ^^^^^^^^
  ```

- Warning: `workflows/original_local.nf:92:3`: Variable was declared but not used

  ```nextflow
    varcalls_l = CLAIR3_CUSTOM(
    ^^^^^^^^^^
  ```

- Warning: `workflows/original_local.nf:113:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .join(ch_samples.map { meta, reads, platform -> tuple(meta, platform) }, by: 0)
                                   ^^^^^
  ```

- Warning: `workflows/original_local.nf:114:15`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .filter { meta, reads, platform ->
                ^^^^
  ```

- Warning: `workflows/original_local.nf:114:21`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .filter { meta, reads, platform ->
                      ^^^^^
  ```

- Warning: `workflows/original_local.nf:117:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .map { meta, reads, platform ->
                          ^^^^^^^^
  ```

- Warning: `workflows/original_local.nf:150:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                            .map { meta, ref, fai_meta, fai -> tuple(meta, ref, fai) }
                                              ^^^^^^^^
  ```

- Warning: `workflows/original_local.nf:156:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
    ch_multiqc_input = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `workflows/original_local.nf:158:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_fastqc_out.collect { meta, files -> files },
                                  ^^^^
  ```

- Warning: `workflows/original_local.nf:159:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_bbduk_stats.collect { meta, files -> files },
                                   ^^^^
  ```

- Warning: `workflows/original_local.nf:160:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_bbduk_logs.collect { meta, files -> files },
                                  ^^^^
  ```

- Warning: `workflows/original_local.nf:161:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_bbduk_dropped.collect { meta, files -> files },
                                     ^^^^
  ```

- Warning: `workflows/original_local.nf:162:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_mm2stats.stats.collect { meta, files -> files },
                                      ^^^^
  ```

- Warning: `workflows/original_local.nf:163:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_bm3stats.stats.collect { meta, files -> files }
                                      ^^^^
  ```

- Warning: `workflows/prepare_references.nf:15:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_queryref = Channel.of(queryurl)
                    ^^^^^^^
  ```

- Warning: `workflows/prepare_references.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_hostref  = Channel.of(hosturl)
                    ^^^^^^^
  ```

- Warning: `workflows/preprocess_reads.nf:16:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_samples = Channel.fromPath(samplesheet)
                   ^^^^^^^
  ```

- Warning: `workflows/preprocess_reads.nf:29:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_reads_raw = ch_samples.map { meta, reads, platform ->
                                                   ^^^^^^^^
  ```

- Warning: `workflows/preprocess_reads.nf:39:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_adapters = Channel.fromPath(adapters)
                    ^^^^^^^
  ```
