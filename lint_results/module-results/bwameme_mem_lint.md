# Nextflow lint results

- Generated: 2026-02-07T00:24:15.163984+00:00
- Nextflow version: 25.12.0-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `modules/nf-core/bwameme/mem/main.nf:75:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/bwameme/mem/main.nf:78:9`: Variable was declared but not used

  ```nextflow
      def samtools_command = sort_bam ? 'sort' : 'view'
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/bwameme/mem/main.nf:82:9`: Variable was declared but not used

  ```nextflow
      def reference = fasta && extension=="cram"  ? "--reference ${fasta}" : ""
          ^^^^^^^^^^
  ```
