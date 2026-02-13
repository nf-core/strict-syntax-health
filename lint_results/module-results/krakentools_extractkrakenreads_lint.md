# Nextflow lint results

- Generated: 2026-02-13T00:24:57.236435+00:00
- Nextflow version: 26.01.1-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `modules/nf-core/krakentools/extractkrakenreads/main.nf:55:9`: Variable was declared but not used

  ```nextflow
      def input_reads_command = meta.single_end ? "-s $classified_reads_fastq" : "-s1 ${classified_reads_fastq[0]} -s2 ${classified_reads_fastq[1]}"
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/krakentools/extractkrakenreads/main.nf:56:9`: Variable was declared but not used

  ```nextflow
      def output_reads_command = meta.single_end ? "-o ${prefix}.extracted_kraken2_read.${extension}" : "-o ${prefix}.extracted_kraken2_read_1.${extension} -o2 ${prefix}.extracted_kraken2_read_2.${extension}"
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/krakentools/extractkrakenreads/main.nf:58:9`: Variable was declared but not used

  ```nextflow
      def report_option = report ? "-r ${report}" : ""
          ^^^^^^^^^^
  ```
