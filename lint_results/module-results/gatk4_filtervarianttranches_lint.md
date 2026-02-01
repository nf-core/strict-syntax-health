# Nextflow lint results

- Generated: 2026-02-01T00:22:15.914544+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/gatk4/filtervarianttranches/main.nf:29:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def resource_list = resources.collect { "--resource ${it}" }.join(' ')
                                                            ^^^^^^^^^^
  ```
