# Nextflow lint results

- Generated: 2026-09-12T00:18:50.690927079Z
- Nextflow version: 26.08.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/local/channel_fastq_create_csv/main.nf:17:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              items.each { allKeys.addAll(it.keySet()) }
                                          ^^
  ```

- Warning: `workflows/demultiplex.nf:193:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      [meta, files.findAll { it.size() > 100 }]  // skip empty fastq files i.e. Undetermined_*.fastq.gz in case no indexes were used for sequencing
                                             ^^
  ```
