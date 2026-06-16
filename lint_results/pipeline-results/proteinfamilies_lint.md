# Nextflow lint results

- Generated: 2026-06-16T14:28:02.457345274Z
- Nextflow version: 26.04.3
- Summary: 7 warnings

## :warning: Warnings

- Warning: `subworkflows/local/align_sequences/main.nf:30:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      alignments = ch_alignments
      ^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nextflow_pipeline/main.nf:43:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:20:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      valid_config = valid_config
      ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:76:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/proteinfamilies.nf:224:88`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(FAA_SEQFU_SEQKIT.out.multiqc_files.collect{it[1]}.ifEmpty([]))
                                                                                         ^^
  ```

- Warning: `workflows/proteinfamilies.nf:225:92`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(CALCULATE_CLUSTER_DISTRIBUTION.out.mqc.collect{it[1]}.ifEmpty([]))
                                                                                             ^^
  ```

- Warning: `workflows/proteinfamilies.nf:226:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(ch_family_reps.collect { it[1] }.ifEmpty([]))
                                                                       ^^
  ```
