# Nextflow lint results

- Generated: 2026-02-02T00:20:06.595381+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/fasta_vclust_prefilter_align_cluster/main.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^^^^
  ```
