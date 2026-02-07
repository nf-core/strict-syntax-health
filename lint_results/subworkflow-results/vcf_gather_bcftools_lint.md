# Nextflow lint results

- Generated: 2026-02-07T00:24:27.406373+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 error

## :x: Errors

- Error: `subworkflows/nf-core/vcf_gather_bcftools/main.nf:14:79`: Unexpected input: '['

  ```nextflow
      if (!(arr_common_meta instanceof List || arr_common_meta instanceof Object[])) {
                                                                                ^^^^^^
  ```
