# Nextflow lint results

- Generated: 2026-05-06T00:37:13.762180647Z
- Nextflow version: 26.04.0
- Summary: 1 error, 1 warning

## :x: Errors

- Error: `workflows/scnanoseq.nf:560:65`: `ch_versions_yaml` is not defined

  ```nextflow
              ch_multiqc_rawqc_files = ch_multiqc_rawqc_files.mix(ch_versions_yaml.collect())
                                                                  ^^^^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```
