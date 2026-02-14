# Nextflow lint results

- Generated: 2026-02-14T00:22:50.971539+00:00
- Nextflow version: 26.01.1-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/nf-core/quantify_rsem/main.nf:46:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
            ch_counts_gene.collect{ it[1] }.map { results -> [ ['id': 'all_samples'], results ] },
                                    ^^^^^^^^^^
    ```

- Warning: `subworkflows/nf-core/quantify_rsem/main.nf:47:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
            ch_counts_transcript.collect{ it[1] }
                                          ^^^^^^^
    ```
