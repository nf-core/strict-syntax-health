# Nextflow lint results

- Generated: 2026-02-02T00:20:06.586818+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 error

## :x: Errors

- Error: `subworkflows/nf-core/bam_split_by_region/main.nf:29:44`: Unexpected input: '='

  ```nextflow
              if (! stats['start'] ) [ chrom = stats['seq_name'] ]
                                             ^^^^^^^^^^
  ```
