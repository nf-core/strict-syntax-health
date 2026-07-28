# Nextflow lint results

- Generated: 2026-07-28T00:32:07.043580846Z
- Nextflow version: 26.07.0-edge
- Summary: 3 warnings

## :warning: Warnings

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
