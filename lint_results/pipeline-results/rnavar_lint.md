# Nextflow lint results

- Generated: 2026-06-04T00:51:16.186472474Z
- Nextflow version: 26.04.3
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
