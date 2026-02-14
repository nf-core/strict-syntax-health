# Nextflow lint results

- Generated: 2026-02-14T00:22:50.958971+00:00
- Nextflow version: 26.01.1-edge
- Summary: 5 warnings

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_taps_conversion/main.nf:21:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_rastair_mbias = Channel.empty()
                         ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_taps_conversion/main.nf:22:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_rastair_call  = Channel.empty()
                         ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_taps_conversion/main.nf:23:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions      = Channel.empty()
                         ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_taps_conversion/main.nf:47:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_rastair_mbiasparser.map{ meta, nOT_clip, nOB_clip -> [ meta, nOT_clip ] },
                                                      ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_taps_conversion/main.nf:48:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_rastair_mbiasparser.map{ meta, nOT_clip, nOB_clip -> [ meta, nOB_clip ] },
                                            ^^^^^^^^^^
  ```
