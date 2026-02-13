# Nextflow lint results

- Generated: 2026-02-13T00:24:57.301131+00:00
- Nextflow version: 26.01.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/sourmash/compare/main.nf:32:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def sigs = signatures ? "${signatures.sort{it.toString()}.join(' ')}" : ''
                                                 ^^^^^^^^^^
  ```
