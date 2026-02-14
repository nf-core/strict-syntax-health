# Nextflow lint results

- Generated: 2026-02-14T00:22:37.794522+00:00
- Nextflow version: 26.01.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/vg/construct/main.nf:28:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      input_files = mode == 'vcf' ? input.collect { "--vcf ${it}" }.join(" ") : "--msa ${input}"
                                                             ^^^^^^^^^^
  ```
