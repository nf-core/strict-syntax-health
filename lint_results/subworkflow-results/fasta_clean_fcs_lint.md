# Nextflow lint results

- Generated: 2026-02-13T00:25:10.835057+00:00
- Nextflow version: 26.01.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/fasta_clean_fcs/main.nf:12:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^^^^
  ```
