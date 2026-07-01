# Nextflow lint results

- Generated: 2026-07-01T00:44:52.789692984Z
- Nextflow version: 26.05.0-edge
- Summary: 23 warnings

## :warning: Warnings

- Warning: `modules/local/dorado/aligner/main.nf:36:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/dorado/polish/main.nf:34:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/merqury/merqury/main.nf:59:9`: Variable was declared but not used

  ```nextflow
      def VERSION = 1.3 // WARN: Version information not provided by tool on CLI. Please update this string when bumping container versions.
          ^^^^^^^
  ```

- Warning: `modules/nf-core/meryl/unionsum/main.nf:35:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/liftoff/main.nf:10:5`: Variable was declared but not used

  ```nextflow
      lifted_annotations = LIFTOFF.out.gff3
      ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/liftoff/main.nf:13:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      lifted_annotations
      ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare/jellyfish/main.nf:93:5`: Variable was declared but not used

  ```nextflow
      genomescope_summary = GENOMESCOPE.out.summary
      ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare/jellyfish/main.nf:95:5`: Variable was declared but not used

  ```nextflow
      genomescope_plot = GENOMESCOPE.out.plot_log
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare/main.nf:83:5`: Variable was declared but not used

  ```nextflow
      meryl_kmers = SHORTREADS.out.meryl_kmers
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare/main.nf:233:5`: Variable was declared but not used

  ```nextflow
      genomescope_summary = JELLYFISH.out.genomescope_summary
      ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare/main.nf:235:5`: Variable was declared but not used

  ```nextflow
      genomescope_plot = JELLYFISH.out.genomescope_plot
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare/main.nf:237:5`: Variable was declared but not used

  ```nextflow
      fastplong_json_reports = HIFI.out.fastplong_hifi_reports.mix(ONT.out.fastplong_ont_reports)
      ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare/prepare_ont/collect/main.nf:18:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      reads
      ^^^^^
  ```

- Warning: `subworkflows/local/prepare/prepare_shortreads/main.nf:173:5`: Variable was declared but not used

  ```nextflow
      meryl_kmers = MERYL_UNIONSUM.out.meryl_db
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/scaffold/main.nf:179:5`: Variable was declared but not used

  ```nextflow
      scaffold_busco_reports = links_busco
      ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/scaffold/main.nf:184:5`: Variable was declared but not used

  ```nextflow
      scaffold_quast_reports = links_quast
      ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/scaffold/main.nf:189:5`: Variable was declared but not used

  ```nextflow
      scaffold_merqury_reports = links_merqury
      ^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_genomeassembler_pipeline/main.nf:33:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
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

- Warning: `workflows/genomeassembler.nf:110:5`: Variable was declared but not used

  ```nextflow
      ch_main_scaffolded = ch_main_polished_branched
      ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/genomeassembler.nf:222:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      _report
      ^^^^^^^
  ```
