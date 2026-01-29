# Nextflow lint results

- Generated: 2026-01-29T00:23:01.574578+00:00
- Nextflow version: 25.12.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_docounts_contamination_angsd/main.nf:15:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_docounts_contamination_angsd/main.nf:17:37`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ANGSD_DOCOUNTS ( ch_bam.combine(Channel.of([[]])) )
                                      ^^^^^^^^^^
  ```
