# Nextflow lint results

- Generated: 2026-02-12T00:24:35.879688+00:00
- Nextflow version: 26.01.1-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/nf-core/fastq_sanitise_seqkit/main.nf:10:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_sanitise_seqkit/main.nf:38:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              def clean_meta = meta.findAll { key, value -> key != 'strandness' }
                                                   ^^^^^^^^^^
  ```
