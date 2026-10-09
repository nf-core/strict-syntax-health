# Nextflow lint results

- Generated: 2026-10-09T00:28:17.652640022Z
- Nextflow version: 26.09.2-edge
- Summary: 3 warnings

## :warning: Warnings

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
