# Nextflow lint results

- Generated: 2026-02-09T00:23:26.107945+00:00
- Nextflow version: 26.01.0-edge
- Summary: 2 errors

## :x: Errors

- Error: `modules/nf-core/cellrangerarc/count/main.nf:8:5`: Invalid process directive

  ```nextflow
      if (workflow.profile.tokenize(',').intersect(['conda', 'mamba']).size() >= 1) {
      ^^^^^^^^^^
  ```

- Error: `modules/nf-core/cellrangerarc/count/tests/nextflow.config:2:33`: Unexpected input: ':'

  ```nextflow
  	withName: 'CELLRANGERARC_COUNT': {
                                  ^^^
  ```
