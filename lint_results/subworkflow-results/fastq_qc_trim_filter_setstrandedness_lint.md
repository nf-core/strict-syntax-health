# Nextflow lint results

- Generated: 2026-04-21T00:34:47.928994+00:00
- Nextflow version: 26.03.3-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/main.nf:426:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { row -> [row[0], row.drop(1).findAll { it != null }.collectMany { e -> (e instanceof List) ? e : [e] }] }
                                                       ^^^^^^^^^^
  ```
