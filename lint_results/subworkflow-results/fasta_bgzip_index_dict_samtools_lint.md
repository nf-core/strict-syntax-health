# Nextflow lint results

- Generated: 2026-06-23T00:45:59.463558+00:00
- Nextflow version: 26.05.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/fasta_bgzip_index_dict_samtools/main.nf:35:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      fasta_fai_gzi_dict = ch_joined             // channel: [ val(meta),  fasta.gz, fai, gzi, sizes, dict ]
      ^^^^^^^^^^
  ```
