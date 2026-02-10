# Nextflow lint results

- Generated: 2026-02-10T00:27:13.423751+00:00
- Nextflow version: 26.01.0-edge
- Summary: 1 error

## :x: Errors

- Error: `subworkflows/nf-core/vcf_gather_bcftools/main.nf:14:79`: Unexpected input: '['

  ```nextflow
      if (!(arr_common_meta instanceof List || arr_common_meta instanceof Object[])) {
                                                                                ^^^^^^
  ```
