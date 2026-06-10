# Nextflow lint results

- Generated: 2026-06-10T00:43:52.407607212Z
- Nextflow version: 26.04.3
- Summary: 12 warnings

## :warning: Warnings

- Warning: `modules/local/cometconfig/main.nf:59:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/ms2rescore/runms2rescore/main.nf:24:5`: Variable was declared but not used

  ```nextflow
      spectra_file = mzml ?: raw_spectra
      ^^^^^^^^^^^^
  ```

- Warning: `modules/local/ms2rescore/runms2rescore/main.nf:25:5`: Variable was declared but not used

  ```nextflow
      ms2pip_model = meta.ms2pip_model ?: 'HCD'
      ^^^^^^^^^^^^
  ```

- Warning: `modules/local/ms2rescore/runms2rescore/main.nf:26:5`: Variable was declared but not used

  ```nextflow
      spectrum_id_pattern = meta.spectrum_id_pattern ?: '.*scan=(\\d+)$'
      ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/ms2rescore/runms2rescore/main.nf:27:5`: Variable was declared but not used

  ```nextflow
      fragment_tol_da = meta.fragment_tol_da ?: 0.02
      ^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/ms2rescore/runms2rescore/main.nf:28:5`: Variable was declared but not used

  ```nextflow
      chunk_size = task.ext.chunk_size ?: 100000
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mspepid_pipeline/main.nf:134:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { validateInputSamplesheet(it) }
                                          ^^
  ```

- Warning: `subworkflows/nf-core/utils_nextflow_pipeline/main.nf:43:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:20:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      valid_config = valid_config
      ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:72:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/mspepid.nf:121:9`: Variable was declared but not used

  ```nextflow
      def ch_collated_versions = softwareVersionsToYAML(ch_versions.mix(topic_versions.versions_file))
          ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/mspepid.nf:130:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions       = ch_versions                 // channel: [ path(versions.yml) ]
      ^^^^^^^^^^^^^^^^^^^^
  ```
