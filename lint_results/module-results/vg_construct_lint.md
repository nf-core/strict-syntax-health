# Nextflow lint results

- Generated: 2026-02-13T00:24:57.317062+00:00
- Nextflow version: 26.01.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/vg/construct/main.nf:28:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      input_files = mode == 'vcf' ? input.collect { "--vcf ${it}" }.join(" ") : "--msa ${input}"
                                                             ^^^^^^^^^^
  ```
