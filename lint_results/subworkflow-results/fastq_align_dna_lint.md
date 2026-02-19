# Nextflow lint results

- Generated: 2026-02-19T00:25:12.763798+00:00
- Nextflow version: 26.01.1-edge
- Summary: 3 warnings

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
