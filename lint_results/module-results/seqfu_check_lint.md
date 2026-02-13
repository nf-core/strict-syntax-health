# Nextflow lint results

- Generated: 2026-02-13T00:24:57.293721+00:00
- Nextflow version: 26.01.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/seqfu/check/main.nf:24:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def dirFlag = (reads instanceof List ? reads.every { it.isDirectory() } : reads.isDirectory()) ? "--dir" : ""
                                                           ^^^^^^^^^^
  ```
