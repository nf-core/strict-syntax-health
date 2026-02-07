# Nextflow lint results

- Generated: 2026-02-07T00:24:15.167709+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 error

## :x: Errors

- Error: `modules/nf-core/cellrangeratac/mkfastq/main.nf:7:5`: Invalid process directive

  ```nextflow
      if (workflow.profile.tokenize(',').intersect(['conda', 'mamba']).size() >= 1) {
      ^^^^^^^^^^
  ```
