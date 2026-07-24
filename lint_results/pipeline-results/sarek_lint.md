# Nextflow lint results

- Generated: 2026-07-24T00:28:45.587154373Z
- Nextflow version: 26.07.0-edge
- Summary: 6 warnings

## :warning: Warnings

- Warning: `modules/nf-core/cnvkit/batch/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def tumor_bam = tumor_exists && tumor.Extension == "bam" ? true : false
          ^^^^^^^^^
  ```

- Warning: `modules/nf-core/cnvkit/batch/main.nf:41:9`: Variable was declared but not used

  ```nextflow
      def normal_bam = normal_exists && normal.Extension == "bam" ? true : false
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/goleft/indexcov/main.nf:31:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_files = bams.findAll{it.name.endsWith(".bam")} + indexes.findAll{it.name.endsWith(".crai")}
                                     ^^
  ```

- Warning: `modules/nf-core/goleft/indexcov/main.nf:31:80`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_files = bams.findAll{it.name.endsWith(".bam")} + indexes.findAll{it.name.endsWith(".crai")}
                                                                                 ^^
  ```

- Warning: `modules/nf-core/goleft/indexcov/main.nf:32:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def extranormalize = input_files.any{it.name.endsWith(".crai")} ? " --extranormalize " : ""
                                           ^^
  ```

- Warning: `modules/nf-core/goleft/indexcov/main.nf:52:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```
