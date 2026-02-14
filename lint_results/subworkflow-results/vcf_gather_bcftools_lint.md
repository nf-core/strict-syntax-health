# Nextflow lint results

- Generated: 2026-02-14T00:22:50.973141+00:00
- Nextflow version: 26.01.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/vcf_gather_bcftools/main.nf:35:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  m.findAll { k, v -> !(k in arr_common_meta) }
                                 ^^^^^^^^^^
  ```
