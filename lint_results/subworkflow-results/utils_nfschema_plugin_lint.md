# Nextflow lint results

- Generated: 2026-10-04T01:03:13.642232+00:00
- Nextflow version: 26.09.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:12:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input_workflow      // workflow: the workflow object used by nf-schema to get metadata from the workflow
      ^^^^^^^^^^
  ```
