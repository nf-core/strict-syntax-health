# Nextflow lint results

- Generated: 2026-07-21T00:28:35.847366687Z
- Nextflow version: 26.07.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `workflows/daamicrobiome.nf:19:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_samplesheet // channel: samplesheet read in from --input
      ^^^^^^^^^^^^^^
  ```

- Warning: `workflows/daamicrobiome.nf:46:9`: Variable was declared but not used

  ```nextflow
      def ch_collated_versions = softwareVersionsToYAML(ch_versions.mix(topic_versions.versions_file))
          ^^^^^^^^^^^^^^^^^^^^
  ```
