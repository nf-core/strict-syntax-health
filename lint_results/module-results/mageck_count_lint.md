# Nextflow lint results

- Generated: 2026-02-12T00:24:23.147808+00:00
- Nextflow version: 26.01.1-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `modules/nf-core/mageck/count/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/mageck/count/main.nf:46:9`: Variable was declared but not used

  ```nextflow
      def input_file = ("$inputfile".endsWith(".fastq.gz")) ? "--fastq ${inputfile}" : "-k ${inputfile}"
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/mageck/count/main.nf:47:9`: Variable was declared but not used

  ```nextflow
      def sample_label = ("$inputfile".endsWith(".fastq.gz") || "$inputfile".endsWith(".fq.gz")) ? "--sample-label ${meta.id}" : ''
          ^^^^^^^^^^
  ```
