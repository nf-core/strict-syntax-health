# Nextflow lint results

- Generated: 2026-11-03T00:13:20.495512925Z
- Nextflow version: 26.10.5
- Summary: 24 warnings

## :warning: Warnings

- Warning: `modules/local/cometconfig/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/cometconfig/main.nf:59:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/fdrbench/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/ms2rescore/getmodel/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/ms2rescore/runms2rescore/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
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

- Warning: `modules/local/psmutilsconversions/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/sagebeta/main.nf:27:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/sageconfig/main.nf:25:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/tdf2mzml/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/comet/main.nf:25:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gunzip/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/openms/decoydatabase/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/percolator/main.nf:26:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/thermorawfileparser/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/untar/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/unzip/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/unzipfiles/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mspepid_pipeline/main.nf:135:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { validateInputSamplesheet(it) }
                                          ^^
  ```

- Warning: `workflows/mspepid.nf:121:9`: Variable was declared but not used

  ```nextflow
      def ch_collated_versions = softwareVersionsToYAML(ch_versions.mix(topic_versions.versions_file))
          ^^^^^^^^^^^^^^^^^^^^
  ```
