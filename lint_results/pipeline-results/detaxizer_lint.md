# Nextflow lint results

- Generated: 2026-10-24T00:19:17.948609241Z
- Nextflow version: 26.10.3
- Summary: 34 warnings

## :warning: Warnings

- Warning: `modules/local/filter/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/filter_blastn_identcov/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/isolate_bbduk_ids/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/isolate_kraken2_ids/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/kraken2preparation/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/map_kraken2seqids_to_fqheaders/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/merge_ids/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/normalize_bbmap_ids/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/parse_kraken2report/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/prepare_fasta4blastn/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/rename_fastq_headers_after/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/rename_fastq_headers_pre/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/summarizer/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/summary_blastn/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/summary_classification/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bbmap/bbduk/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bbmap/filterbyname/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/blast/blastn/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/blast/makeblastdb/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/fastp/main.nf:25:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/fastqc/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:24:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/multiqc/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `subworkflows/local/generate_downstream_samplesheets/main.nf:106:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              se: it.short_reads_2 ==""
                  ^^
  ```

- Warning: `subworkflows/local/generate_downstream_samplesheets/main.nf:124:15`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map{ it.keySet().join(format_sep) }
                ^^
  ```

- Warning: `subworkflows/local/generate_downstream_samplesheets/main.nf:125:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .concat( ch_list_for_samplesheet.map{ it.values().join(format_sep) })
                                                ^^
  ```

- Warning: `workflows/detaxizer.nf:83:21`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          shortReads: it[1]
                      ^^
  ```

- Warning: `workflows/detaxizer.nf:85:57`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          meta, short_reads_fastq_1, short_reads_fastq_2, long_reads_fastq_1 ->
                                                          ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/detaxizer.nf:94:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          longReads: it[3]
                     ^^
  ```

- Warning: `workflows/detaxizer.nf:96:15`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          meta, short_reads_fastq_1, short_reads_fastq_2, long_reads_fastq_1 ->
                ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/detaxizer.nf:96:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          meta, short_reads_fastq_1, short_reads_fastq_2, long_reads_fastq_1 ->
                                     ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/detaxizer.nf:185:75`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_parsed_kraken2_report = PARSE_KRAKEN2REPORT.out.to_filter.map {meta, path -> path}
                                                                            ^^^^
  ```

- Warning: `workflows/detaxizer.nf:274:13`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, path -> [path]
              ^^^^
  ```

- Warning: `workflows/detaxizer.nf:389:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, path -> [path]
                  ^^^^
  ```
