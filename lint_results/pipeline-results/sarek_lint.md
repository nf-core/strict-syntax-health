# Nextflow lint results

- Generated: 2026-07-23T00:32:57.476258501Z
- Nextflow version: 26.07.0-edge
- Summary: 21 warnings

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

- Warning: `modules/nf-core/lofreq/callparallel/main.nf:29:9`: Variable was declared but not used

  ```nextflow
      def alignment_bam = bam.Extension == "bam" ? true : false
          ^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/manta/germline/main.nf:33:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_files = input.collect{"--bam ${it}"}.join(' ')
                                               ^^
  ```

- Warning: `modules/nf-core/svdb/merge/main.nf:38:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def pairs = vcfs.indices.collect { [vcfs[it], input_priority[it]] }
                                                      ^^
  ```

- Warning: `modules/nf-core/svdb/merge/main.nf:38:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def pairs = vcfs.indices.collect { [vcfs[it], input_priority[it]] }
                                                                          ^^
  ```

- Warning: `modules/nf-core/svdb/merge/main.nf:40:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              vcfs = pairs.collect { it[0] }
                                     ^^
  ```

- Warning: `modules/nf-core/svdb/merge/main.nf:41:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              priority = pairs.collect { it[1] }
                                         ^^
  ```

- Warning: `modules/nf-core/svdb/merge/main.nf:55:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          input = (vcfs.collect().size() > 1 && sort_inputs) ? vcfs.sort { it.name } : vcfs
                                                                           ^^
  ```

- Warning: `modules/nf-core/vcftools/main.nf:97:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      args_list.removeIf { it.contains('--bed') }
                           ^^
  ```

- Warning: `modules/nf-core/vcftools/main.nf:98:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      args_list.removeIf { it.contains('--exclude-bed') }
                           ^^
  ```

- Warning: `modules/nf-core/vcftools/main.nf:99:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      args_list.removeIf { it.contains('--hapcount') }
                           ^^
  ```

- Warning: `modules/nf-core/vcftools/main.nf:100:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      args_list.removeIf { it.contains('--positions') }
                           ^^
  ```

- Warning: `modules/nf-core/vcftools/main.nf:101:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      args_list.removeIf { it.contains('--exclude-positions') }
                           ^^
  ```

- Warning: `modules/nf-core/vcftools/main.nf:106:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      args_list.removeIf { it.contains('--diff') }
                           ^^
  ```

- Warning: `modules/nf-core/vcftools/main.nf:107:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      args_list.removeIf { it.contains('--gzdiff') }
                           ^^
  ```

- Warning: `modules/nf-core/vcftools/main.nf:108:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      args_list.removeIf { it.contains('--diff-bcf') }
                           ^^
  ```
