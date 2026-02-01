# Nextflow lint results

- Generated: 2026-02-01T00:22:15.914694+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/gatk4/gatherbqsrreports/main.nf:23:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = table.collect { "--input ${it}" }.join(' ')
                                                  ^^^^^^^^^^
  ```
