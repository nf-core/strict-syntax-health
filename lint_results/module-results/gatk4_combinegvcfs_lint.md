# Nextflow lint results

- Generated: 2026-02-02T00:19:53.378325+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/gatk4/combinegvcfs/main.nf:26:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = vcf.collect { "--variant ${it}" }.join(' ')
                                                  ^^^^^^^^^^
  ```
