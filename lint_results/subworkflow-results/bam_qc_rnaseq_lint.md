# Nextflow lint results

- Generated: 2026-04-21T00:34:47.921831+00:00
- Nextflow version: 26.03.3-edge
- Summary: 4 warnings

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_qc_rnaseq/main.nf:25:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def rseqc_modules = tools.findAll { it.startsWith('rseqc_') }.collect { it.replace('rseqc_', '') }
                                          ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_qc_rnaseq/main.nf:25:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def rseqc_modules = tools.findAll { it.startsWith('rseqc_') }.collect { it.replace('rseqc_', '') }
                                                                              ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_qc_rnaseq/main.nf:85:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_qc_rnaseq/main.nf:113:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { row -> [row[0], row.drop(1).findAll { it != null }.collectMany { e -> (e instanceof List) ? e : [e] }] }
                                                       ^^^^^^^^^^
  ```
