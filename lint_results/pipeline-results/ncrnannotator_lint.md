# Nextflow lint results

- Generated: 2026-11-05T00:13:46.233063218Z
- Nextflow version: 26.10.5
- Summary: 4 warnings

## :warning: Warnings

- Warning: `modules/nf-core/multiqc/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_ncrnannotator_pipeline/main.nf:184:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              errors.collect { "    * ${it}" }.join("\n") + "\n" +
                                        ^^
  ```

- Warning: `workflows/ncrnannotator.nf:96:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          CMSEARCH.out.tblout.collect { it[1] },
                                        ^^
  ```

- Warning: `workflows/ncrnannotator.nf:111:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```
