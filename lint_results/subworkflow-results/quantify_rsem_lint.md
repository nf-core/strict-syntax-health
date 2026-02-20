# Nextflow lint results

- Generated: 2026-02-20T00:23:00.646989+00:00
- Nextflow version: 26.01.1-edge
- Summary: 2 errors

## :x: Errors

- Error: `subworkflows/nf-core/quantify_rsem/main.nf:46:33`: `index` is already declared

  ```nextflow
          ch_counts_gene.collect{ index -> index[1] }.map { results -> [ ['id': 'all_samples'], results ] },
                                  ^^^^^^^^^^
  ```

- Error: `subworkflows/nf-core/quantify_rsem/main.nf:47:39`: `index` is already declared

  ```nextflow
          ch_counts_transcript.collect{ index -> index[1] }
                                        ^^^^^^^^^^
  ```
