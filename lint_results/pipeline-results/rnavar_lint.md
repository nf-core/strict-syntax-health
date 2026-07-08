# Nextflow lint results

- Generated: 2026-07-08T00:29:45.810415256Z
- Nextflow version: 26.06.0-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `subworkflows/local/prepare_alignment/main.nf:25:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      reads_index = input_reads.indexed.mix(input_reads.not_indexed.join(SAMTOOLS_INDEX.out.index, failOnMismatch: true, failOnDuplicate: true)) // [ val(meta), path(bam|cram), path(bai|crai) ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/recalibrate/main.nf:33:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      bam = bam_recalibrated_index
      ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/splitncigar/main.nf:52:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      bam_bai = SAMTOOLS_MERGE.out.bam.join(SAMTOOLS_INDEX.out.index, failOnDuplicate: true, failOnMismatch: true)
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```
