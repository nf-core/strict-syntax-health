# Nextflow lint results

- Generated: 2026-02-14T00:22:50.968574+00:00
- Nextflow version: 26.01.1-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/nf-core/fastq_index_filter_deacon/main.nf:12:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map  { meta, fasta, reads -> [ meta, fasta ] }
                               ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_index_filter_deacon/main.nf:15:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map  { meta, fasta, reads ->
                        ^^^^^^^^^^
  ```
