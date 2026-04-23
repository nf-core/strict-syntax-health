# Nextflow lint results

- Generated: 2026-04-23T00:36:45.929450+00:00
- Nextflow version: 26.03.3-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_dedup_umi/main.nf:129:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { row -> [row[0], row.drop(1).findAll { it != null }.collectMany { e -> (e instanceof List) ? e : [e] }] }
                                                       ^^^^^^^^^^
  ```
