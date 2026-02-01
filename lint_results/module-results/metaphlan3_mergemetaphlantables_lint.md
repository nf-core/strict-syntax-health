# Nextflow lint results

- Generated: 2026-02-01T00:22:15.953175+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/metaphlan3/mergemetaphlantables/main.nf:22:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input = profiles.sort{it.toString()}.join(" ")
                                ^^^^^^^^^^
  ```
