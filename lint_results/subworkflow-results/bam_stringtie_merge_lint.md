# Nextflow lint results

- Generated: 2026-02-13T00:25:10.829828+00:00
- Nextflow version: 26.01.1-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_stringtie_merge/main.nf:12:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions       = Channel.empty()
                          ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_stringtie_merge/main.nf:13:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_stringtie_gtfs = Channel.empty()
                          ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_stringtie_merge/main.nf:21:16`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { it[1] }
                 ^^^^^^^
  ```
