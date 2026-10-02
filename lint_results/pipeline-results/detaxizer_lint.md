# Nextflow lint results

- Generated: 2026-10-02T00:21:15.198002717Z
- Nextflow version: 26.09.1-edge
- Summary: 21 warnings

## :warning: Warnings

- Warning: `subworkflows/local/generate_downstream_samplesheets/main.nf:73:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter{ it.short_reads_1!="" } // MAG doesn't support standalone long reads
                   ^^
  ```

- Warning: `subworkflows/local/generate_downstream_samplesheets/main.nf:75:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              se: it.short_reads_2 ==""
                  ^^
  ```

- Warning: `subworkflows/local/generate_downstream_samplesheets/main.nf:81:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter{ it.long_reads !="" && it.short_reads_1=="" }
                   ^^
  ```

- Warning: `subworkflows/local/generate_downstream_samplesheets/main.nf:81:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter{ it.long_reads !="" && it.short_reads_1=="" }
                                         ^^
  ```

- Warning: `subworkflows/local/generate_downstream_samplesheets/main.nf:82:169`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .collect{ log.warn("Standalone long reads are not yet supported by the nf-core/mag pipeline and ARE REMOVED from the samplesheet 'mag-{se,pe}.csv' \n sample: ${it.sample}" )}
                                                                                                                                                                          ^^
  ```

- Warning: `subworkflows/local/generate_downstream_samplesheets/main.nf:114:15`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map{ it.keySet().join(format_sep) }
                ^^
  ```

- Warning: `subworkflows/local/generate_downstream_samplesheets/main.nf:115:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .concat( ch_list_for_samplesheet.map{ it.values().join(format_sep) })
                                                ^^
  ```

- Warning: `workflows/detaxizer.nf:82:21`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          shortReads: it[1]
                      ^^
  ```

- Warning: `workflows/detaxizer.nf:84:57`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          meta, short_reads_fastq_1, short_reads_fastq_2, long_reads_fastq_1 ->
                                                          ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/detaxizer.nf:93:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          longReads: it[3]
                     ^^
  ```

- Warning: `workflows/detaxizer.nf:95:15`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          meta, short_reads_fastq_1, short_reads_fastq_2, long_reads_fastq_1 ->
                ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/detaxizer.nf:95:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          meta, short_reads_fastq_1, short_reads_fastq_2, long_reads_fastq_1 ->
                                     ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/detaxizer.nf:184:75`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_parsed_kraken2_report = PARSE_KRAKEN2REPORT.out.to_filter.map {meta, path -> path}
                                                                            ^^^^
  ```

- Warning: `workflows/detaxizer.nf:273:13`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, path -> [path]
              ^^^^
  ```

- Warning: `workflows/detaxizer.nf:388:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, path -> [path]
                  ^^^^
  ```

- Warning: `workflows/detaxizer.nf:427:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ch_to_filter.map { meta, reads, ids -> tuple(meta, reads) },
                                                  ^^^
  ```

- Warning: `workflows/detaxizer.nf:428:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ch_to_filter.map { meta, reads, ids -> ids.toString() },
                                     ^^^^
  ```

- Warning: `workflows/detaxizer.nf:428:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ch_to_filter.map { meta, reads, ids -> ids.toString() },
                                           ^^^^^
  ```

- Warning: `workflows/detaxizer.nf:435:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      ch_to_filter.map { meta, reads, ids -> tuple(meta, reads) },
                                                      ^^^
  ```

- Warning: `workflows/detaxizer.nf:436:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      ch_to_filter.map { meta, reads, ids -> ids.toString() },
                                         ^^^^
  ```

- Warning: `workflows/detaxizer.nf:436:46`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      ch_to_filter.map { meta, reads, ids -> ids.toString() },
                                               ^^^^^
  ```
