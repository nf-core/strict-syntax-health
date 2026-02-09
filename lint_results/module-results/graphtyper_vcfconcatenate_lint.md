# Nextflow lint results

- Generated: 2026-02-09T00:23:26.153972+00:00
- Nextflow version: 26.01.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/graphtyper/vcfconcatenate/main.nf:27:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      input_vcfs = vcf.collate(1000).collect{it.join(' ')} // Batching needed because if there are too many VCFs the shell cannot run the command
                                             ^^^^^^^^^^
  ```
