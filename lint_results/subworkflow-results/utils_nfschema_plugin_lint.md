# Nextflow lint results

- Generated: 2026-10-07T00:25:44.698874+00:00
- Nextflow version: 26.09.2-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:12:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input_workflow      // workflow: the workflow object used by nf-schema to get metadata from the workflow
      ^^^^^^^^^^
  ```
