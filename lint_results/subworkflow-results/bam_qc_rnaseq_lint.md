# Nextflow lint results

- Generated: 2026-04-18T00:30:09.886126+00:00
- Nextflow version: 26.03.2-edge
- Summary: 3 warnings

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
