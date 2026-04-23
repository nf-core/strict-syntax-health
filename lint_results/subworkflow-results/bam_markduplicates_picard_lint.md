# Nextflow lint results

- Generated: 2026-04-23T00:36:45.930030+00:00
- Nextflow version: 26.03.3-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_markduplicates_picard/main.nf:29:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { row -> [row[0], row.drop(1).findAll { it != null }.collectMany { e -> (e instanceof List) ? e : [e] }] }
                                                       ^^^^^^^^^^
  ```
