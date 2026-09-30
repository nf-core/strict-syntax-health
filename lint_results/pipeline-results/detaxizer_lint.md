# Nextflow lint results

- Generated: 2026-09-30T00:22:30.161387763Z
- Nextflow version: 26.09.1-edge
- Summary: 28 warnings

## :warning: Warnings

- Warning: `modules/nf-core/bbmap/bbduk/main.nf:48:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/blast/blastn/main.nf:65:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/blast/makeblastdb/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args           = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:60:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:62:9`: Variable was declared but not used

  ```nextflow
      def paired       = meta.single_end ? "" : "--paired"
          ^^^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:65:9`: Variable was declared but not used

  ```nextflow
      def readclassification_option = save_reads_assignment ? "--output ${prefix}.kraken2.classifiedreads.txt" : "--output /dev/null"
          ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:66:9`: Variable was declared but not used

  ```nextflow
      def compress_reads_command = save_output_fastqs ? "pigz -p $task.cpus *.fastq" : ""
          ^^^^^^^^^^^^^^^^^^^^^^
  ```

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

- Warning: `workflows/detaxizer.nf:189:75`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_parsed_kraken2_report = PARSE_KRAKEN2REPORT.out.to_filter.map {meta, path -> path}
                                                                            ^^^^
  ```

- Warning: `workflows/detaxizer.nf:282:13`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, path -> [path]
              ^^^^
  ```

- Warning: `workflows/detaxizer.nf:403:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, path -> [path]
                  ^^^^
  ```

- Warning: `workflows/detaxizer.nf:443:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ch_to_filter.map { meta, reads, ids -> tuple(meta, reads) },
                                                  ^^^
  ```

- Warning: `workflows/detaxizer.nf:444:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ch_to_filter.map { meta, reads, ids -> ids.toString() },
                                     ^^^^
  ```

- Warning: `workflows/detaxizer.nf:444:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ch_to_filter.map { meta, reads, ids -> ids.toString() },
                                           ^^^^^
  ```

- Warning: `workflows/detaxizer.nf:452:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      ch_to_filter.map { meta, reads, ids -> tuple(meta, reads) },
                                                      ^^^
  ```

- Warning: `workflows/detaxizer.nf:453:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      ch_to_filter.map { meta, reads, ids -> ids.toString() },
                                         ^^^^
  ```

- Warning: `workflows/detaxizer.nf:453:46`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      ch_to_filter.map { meta, reads, ids -> ids.toString() },
                                               ^^^^^
  ```
