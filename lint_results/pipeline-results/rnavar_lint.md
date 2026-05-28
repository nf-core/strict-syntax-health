# Nextflow lint results

- Generated: 2026-05-28T00:38:30.039024469Z
- Nextflow version: 26.04.2
- Summary: 3 warnings

## :warning: Warnings

- Warning: `subworkflows/local/prepare_alignment/main.nf:31:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      reads_index = alignment_out // [ val(meta), path(bam|cram), path(bai|crai) ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/recalibrate/main.nf:33:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      bam = bam_recalibrated_index
      ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/splitncigar/main.nf:55:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      bam_bai = SAMTOOLS_MERGE.out.bam.join(SAMTOOLS_INDEX.out.index, failOnDuplicate: true, failOnMismatch: true)
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```
