# Nextflow lint results

- Generated: 2026-11-13T00:19:31.942562205Z
- Nextflow version: 26.10.5
- Summary: 12 warnings

## :warning: Warnings

- Warning: `modules/nf-core/multiqc/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `subworkflows/local/download_public_datasets/main.nf:24:5`: Variable was declared but not used

  ```nextflow
      ch_fetched_accessions = channel.empty()
      ^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_stableexpression_pipeline/main.nf:33:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_stableexpression_pipeline/main.nf:208:17`: Variable was declared but not used

  ```nextflow
              def nb_candidates_per_section = params.nb_candidates_per_section.toInteger()
                  ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_stableexpression_pipeline/main.nf:210:38`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          catch (NumberFormatException e) {
                                       ^
  ```

- Warning: `subworkflows/local/utils_nfcore_stableexpression_pipeline/main.nf:261:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, file ->
                    ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_stableexpression_pipeline/main.nf:278:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, file ->
                 ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_stableexpression_pipeline/main.nf:407:13`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              it.get(1).size() == 2 // only groups with two files
              ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_stableexpression_pipeline/main.nf:410:13`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, files ->
              ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_stableexpression_pipeline/main.nf:495:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      meta, file -> // extracts design file and adds batch column whenever missing (for custom datasets)
                            ^^^^
  ```

- Warning: `workflows/stableexpression.nf:40:5`: Variable was declared but not used

  ```nextflow
      ch_all_counts                          = channel.empty()
      ^^^^^^^^^^^^^
  ```

- Warning: `workflows/stableexpression.nf:43:5`: Variable was declared but not used

  ```nextflow
      ch_platform_statistics                 = channel.empty()
      ^^^^^^^^^^^^^^^^^^^^^^
  ```
