# Nextflow lint results

- Generated: 2026-06-15T00:46:19.974529+00:00
- Nextflow version: 26.04.3
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/fasta_bgzip_index_dict_samtools/main.nf:35:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      fasta_fai_gzi_dict = ch_joined             // channel: [ val(meta),  fasta.gz, fai, gzi, sizes, dict ]
      ^^^^^^^^^^
  ```
