# Nextflow lint results

- Generated: 2026-04-11T00:25:40.699781118Z
- Nextflow version: 26.03.2-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```

- Warning: `tests/functions/csvToTSV/main.nf:8:5`: Variable was declared but not used

  ```nextflow
      captured = csvToTSV(ch_samplesheet)
      ^^^^^^^^
  ```

- Warning: `tests/functions/generateFastqMeta/main.nf:11:5`: Variable was declared but not used

  ```nextflow
      captured = generateFastqMeta(ch_reads, sample_name_regex, platform, use_sanitized_id)
      ^^^^^^^^
  ```
