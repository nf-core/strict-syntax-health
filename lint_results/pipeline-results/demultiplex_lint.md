# Nextflow lint results

- Generated: 2026-08-22T00:10:11.503221759Z
- Nextflow version: 26.08.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/local/channel_fastq_create_csv/main.nf:17:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              items.each { allKeys.addAll(it.keySet()) }
                                          ^^
  ```
