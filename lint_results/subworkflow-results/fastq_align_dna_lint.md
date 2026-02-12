# Nextflow lint results

- Generated: 2026-02-12T00:24:35.877866+00:00
- Nextflow version: 26.01.1-edge
- Summary: 4 warnings

## :warning: Warnings

- Warning: `subworkflows/nf-core/fastq_align_dna/main.nf:27:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_bam_index    = Channel.empty()
                            ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_align_dna/main.nf:28:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_bam          = Channel.empty()
                            ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_align_dna/main.nf:29:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_reports      = Channel.empty()
                            ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_align_dna/main.nf:30:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_versions     = Channel.empty()
                            ^^^^^^^^^^
  ```
