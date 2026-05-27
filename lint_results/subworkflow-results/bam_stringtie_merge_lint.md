# Nextflow lint results

- Generated: 2026-05-27T00:44:41.089070+00:00
- Nextflow version: 26.04.2
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_stringtie_merge/main.nf:29:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      stringtie_gtf = STRINGTIE_MERGE.out.merged_gtf // channel: [ meta, gtf ]
      ^^^^^^^^^^
  ```
