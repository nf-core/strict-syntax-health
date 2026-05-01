# Nextflow lint results

- Generated: 2026-05-01T00:35:31.712256132Z
- Nextflow version: 26.04.0
- Summary: 7 warnings

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

- Warning: `workflows/mspepid.nf:110:9`: Variable was declared but not used

  ```nextflow
      def ch_collated_versions = softwareVersionsToYAML(ch_versions.mix(topic_versions.versions_file))
          ^^^^^^^^^^^^^^^^^^^^
  ```
