# Nextflow lint results

- Generated: 2026-02-08T00:29:10.362489+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/seqfu/check/main.nf:24:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def dirFlag = (reads instanceof List ? reads.every { it.isDirectory() } : reads.isDirectory()) ? "--dir" : ""
                                                           ^^^^^^^^^^
  ```
