# Nextflow lint results

- Generated: 2026-07-09T00:37:14.333816+00:00
- Nextflow version: 26.06.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_stringtie_merge/main.nf:29:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      stringtie_gtf = STRINGTIE_MERGE.out.merged_gtf // channel: [ meta, gtf ]
      ^^^^^^^^^^
  ```
