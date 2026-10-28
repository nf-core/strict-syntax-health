# Nextflow lint results

- Generated: 2026-10-28T00:15:48.435455478Z
- Nextflow version: 26.10.4
- Summary: 19 warnings

## :warning: Warnings

- Warning: `modules/local/fastq_passthrough/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bbmap/repair/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/fastqc/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/fq/lint/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gzrt/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/multiqc/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/wipertools/fastqgather/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/wipertools/fastqgather/main.nf:25:21`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      if (fastq.any { it.name == "${prefix}.fastq.gz" }) {
                      ^^
  ```

- Warning: `modules/nf-core/wipertools/fastqgather/main.nf:46:21`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      if (fastq.any { it.name == "${prefix}.fastq.gz" }) {
                      ^^
  ```

- Warning: `modules/nf-core/wipertools/fastqscatter/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/wipertools/fastqwiper/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/wipertools/reportgather/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/wipertools/reportgather/main.nf:25:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      if (report.any { it.name == "${prefix}.report" }) {
                       ^^
  ```

- Warning: `modules/nf-core/wipertools/reportgather/main.nf:46:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      if (report.any { it.name == "${prefix}.report" }) {
                       ^^
  ```

- Warning: `subworkflows/local/fastq_repair_wipertools/main.nf:12:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/fastq_repair_wipertools/main.nf:49:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_cleaned_fastq = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/fastq_repair_wipertools/main.nf:54:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def fq = id_fq.sort { a, b -> a[0] <=> b[0] }.collect { it[1] }
                                                                  ^^
  ```

- Warning: `subworkflows/local/fastq_repair_wipertools/main.nf:66:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gathered_report = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/fastq_repair_wipertools/main.nf:74:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_final_reports = Channel.empty()
                         ^^^^^^^
  ```
