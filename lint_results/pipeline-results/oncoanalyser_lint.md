# Nextflow lint results

- Generated: 2026-04-03T00:26:52.322774020Z
- Nextflow version: 26.03.1-edge
- Summary: 64 errors, 102 warnings

## :x: Errors

- Error: `conf/modules.config:314:128`: Unexpected input: '='

  ```nextflow
              saveAs: { filename -> get_saveas_path(meta, task, filename, "panel_resources/${filename}", panel_resource_creation = true) },
                                                                                                                                 ^
  ```

- Error: `main.nf:84:20`: Unexpected input: '='

  ```nextflow
      if (run_mode === Constants.RunMode.PREPARE_REFERENCE)  {
                     ^
  ```

- Error: `modules/local/lilac/main.nf:82:9`: `Sys` is not defined

  ```nextflow
          Sys.exit(1)
          ^^^
  ```

- Error: `modules/local/orange/main.nf:60:39`: Unexpected input: '='

  ```nextflow
      def experiment_type = (run_mode === Constants.RunMode.WGTS) ? 'WGS' : 'PANEL'
                                        ^
  ```

- Error: `modules/local/wisp/main.nf:60:21`: `primary_amber_dir` is not defined

  ```nextflow
          for fp in ${primary_amber_dir}/*.amber.*; do ln -sf ../\$fp amber_dir__prepared/; done
                      ^^^^^^^^^^^^^^^^^
  ```

- Error: `modules/local/wisp/main.nf:61:21`: `sample_amber_dir` is not defined

  ```nextflow
          for fp in ${sample_amber_dir}/*.amber.*;  do ln -sf ../\$fp amber_dir__prepared/; done
                      ^^^^^^^^^^^^^^^^
  ```

- Error: `modules/nf-core/bwa/index/main.nf:15:10`: `bwa_index` is not defined

  ```nextflow
      path bwa_index     , emit: index
           ^^^^^^^^^
  ```

- Error: `subworkflows/local/amber_profiling/main.nf:5:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Constants
  ^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/amber_profiling/main.nf:6:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Utils
  ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/bamtools_metrics/main.nf:5:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Constants
  ^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/bamtools_metrics/main.nf:6:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Utils
  ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/chord_prediction/main.nf:5:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Constants
  ^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/chord_prediction/main.nf:6:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Utils
  ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/cider_calling/main.nf:5:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Constants
  ^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/cider_calling/main.nf:6:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Utils
  ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/cobalt_normalisation/main.nf:5:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Constants
  ^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/cobalt_normalisation/main.nf:6:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Utils
  ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/cobalt_profiling/main.nf:59:49`: Unexpected input: '\*'

  ```nextflow
              ch_inputs_sorted.runnable_tn.map { [*it, []] },
                                                  ^
  ```

- Error: `subworkflows/local/cuppa_prediction/main.nf:46:27`: Unexpected input: '\*'

  ```nextflow
              return [meta, *inputs]
                            ^
  ```

- Error: `subworkflows/local/esvee_calling/main.nf:62:49`: Unexpected input: '\*'

  ```nextflow
              ch_inputs_sorted.runnable_to.map { [*it, [], []] },
                                                  ^
  ```

- Error: `subworkflows/local/isofox_normalisation/main.nf:5:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Constants
  ^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/isofox_normalisation/main.nf:6:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Utils
  ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/isofox_quantification/main.nf:5:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Constants
  ^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/isofox_quantification/main.nf:6:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Utils
  ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/lilac_calling/main.nf:5:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Constants
  ^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/lilac_calling/main.nf:6:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Utils
  ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/linx_annotation/main.nf:5:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Constants
  ^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/linx_annotation/main.nf:6:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Utils
  ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/linx_plotting/main.nf:5:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Constants
  ^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/linx_plotting/main.nf:6:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Utils
  ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/neo_prediction/main.nf:55:27`: Unexpected input: '\*'

  ```nextflow
              return [meta, *inputs]
                            ^
  ```

- Error: `subworkflows/local/orange_reporting/main.nf:125:27`: Unexpected input: '\*'

  ```nextflow
              return [meta, *inputs_selected]
                            ^
  ```

- Error: `subworkflows/local/pave_annotation/main.nf:5:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Constants
  ^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/pave_annotation/main.nf:6:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Utils
  ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/pave_pon_creation/main.nf:5:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Constants
  ^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/pave_pon_creation/main.nf:6:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Utils
  ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/peach_calling/main.nf:5:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Constants
  ^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/peach_calling/main.nf:6:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Utils
  ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/prepare_inputs/main.nf:11:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Utils
  ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/prepare_reference/main.nf:215:28`: Unexpected input: '='

  ```nextflow
              if (run_mode !== Constants.RunMode.PANEL_RESOURCE_CREATION) {
                             ^
  ```

- Error: `subworkflows/local/purple_calling/main.nf:68:27`: Unexpected input: '\*'

  ```nextflow
              return [meta, *inputs]
                            ^
  ```

- Error: `subworkflows/local/read_alignment_dna/main.nf:122:29`: Unexpected input: '\*'

  ```nextflow
                              *:meta_fastq,
                              ^
  ```

- Error: `subworkflows/local/read_alignment_rna/main.nf:65:17`: Unexpected input: '\*'

  ```nextflow
                  *:meta_fastq,
                  ^
  ```

- Error: `subworkflows/local/redux_processing/main.nf:5:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Constants
  ^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/redux_processing/main.nf:6:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Utils
  ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/sage_append/main.nf:36:43`: Unexpected input: '='

  ```nextflow
      def purity_estimate_mode = run_mode === Constants.RunMode.PURITY_ESTIMATE
                                            ^
  ```

- Error: `subworkflows/local/sage_calling/main.nf:5:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Constants
  ^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/sage_calling/main.nf:6:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Utils
  ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/sage_calling/main.nf:8:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import java.nio.channels.Channel
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/sigs_fitting/main.nf:5:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Constants
  ^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/sigs_fitting/main.nf:6:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Utils
  ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/teal_characterisation/main.nf:86:40`: Unexpected input: '\*'

  ```nextflow
          .map { meta, bam_bai -> [meta, *bam_bai] }
                                         ^
  ```

- Error: `subworkflows/local/virusbreakend_calling/main.nf:103:27`: Unexpected input: '\*'

  ```nextflow
              return [meta, *inputs]
                            ^
  ```

- Error: `subworkflows/local/wisp_analysis/main.nf:46:40`: Unexpected input: '='

  ```nextflow
              if (purity_estimate_mode === Constants.RunMode.WGTS) {
                                         ^
  ```

- Error: `workflows/panel_resource_creation.nf:136:54`: Unexpected input: '='

  ```nextflow
      isofox_read_length = params.isofox_read_length !== null ? params.isofox_read_length : Constants.DEFAULT_ISOFOX_READ_LENGTH_TARGETED
                                                       ^
  ```

- Error: `workflows/prepare_reference.nf:1:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Constants
  ^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/prepare_reference.nf:2:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Processes
  ^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/prepare_reference.nf:3:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import Utils
  ^^^^^^^^^^^^
  ```

- Error: `workflows/prepare_reference.nf:11:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/oncoanalyser/subworkflows/local/prepare_reference/main.nf'

  ```nextflow
  include { PREPARE_REFERENCE as STAGE_REFERENCE } from '../subworkflows/local/prepare_reference'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/prepare_reference.nf:28:5`: `STAGE_REFERENCE` is not defined

  ```nextflow
      STAGE_REFERENCE(
      ^^^^^^^^^^^^^^^
  ```

- Error: `workflows/prepare_reference.nf:33:35`: `STAGE_REFERENCE` is not defined

  ```nextflow
      ch_versions = ch_versions.mix(STAGE_REFERENCE.out.versions)
                                    ^^^^^^^^^^^^^^^
  ```

- Error: `workflows/purity_estimate.nf:147:63`: Unexpected input: '='

  ```nextflow
      if (run_config.stages.amber && purity_estimate_run_mode === Constants.RunMode.WGTS) {
                                                                ^
  ```

- Error: `workflows/targeted.nf:182:54`: Unexpected input: '='

  ```nextflow
      isofox_read_length = params.isofox_read_length !== null ? params.isofox_read_length : Constants.DEFAULT_ISOFOX_READ_LENGTH_TARGETED
                                                       ^
  ```

- Error: `workflows/wgts.nf:79:44`: Unexpected input: '='

  ```nextflow
      gridss_config = params.gridss_config !== null ? file(params.gridss_config) : hmf_data.gridss_config
                                             ^
  ```

## :warning: Warnings

- Warning: `modules/local/wisp/main.nf:34:9`: Variable was declared but not used

  ```nextflow
      def purity_estimate_mode = Utils.getEnumFromString(params.purity_estimate_mode, Constants.RunMode)
          ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/gatk4/markduplicates/main.nf:30:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = bam.collect{"--INPUT $it"}.join(' ')
                                            ^^
  ```

- Warning: `modules/nf-core/star/genomegenerate/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def args_list   = args.tokenize()
          ^^^^^^^^^
  ```

- Warning: `subworkflows/local/amber_profiling/main.nf:27:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/amber_profiling/main.nf:50:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai, normal_bam, normal_bai, donor_bam, donor_bai ->
                                     ^^^^^^^^^
  ```

- Warning: `subworkflows/local/amber_profiling/main.nf:50:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai, normal_bam, normal_bai, donor_bam, donor_bai ->
                                                ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/amber_profiling/main.nf:50:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai, normal_bam, normal_bai, donor_bam, donor_bai ->
                                                            ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/amber_profiling/main.nf:50:71`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai, normal_bam, normal_bai, donor_bam, donor_bai ->
                                                                        ^^^^^^^^^
  ```

- Warning: `subworkflows/local/amber_profiling/main.nf:50:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai, normal_bam, normal_bai, donor_bam, donor_bai ->
                                                                                   ^^^^^^^^^
  ```

- Warning: `subworkflows/local/amber_profiling/main.nf:99:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_outputs = Channel.empty()
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/bamtools_metrics/main.nf:27:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/bamtools_metrics/main.nf:40:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, bam, bai ->
                               ^^^
  ```

- Warning: `subworkflows/local/bamtools_metrics/main.nf:57:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, bam, bai ->
                               ^^^
  ```

- Warning: `subworkflows/local/bamtools_metrics/main.nf:66:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_bamtools_inputs = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/bamtools_metrics/main.nf:97:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta_bamtools, metrics_dir ->
                                   ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bamtools_metrics/main.nf:106:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_somatic_metrics_dir = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `subworkflows/local/bamtools_metrics/main.nf:112:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_germline_metrics_dir = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/chord_prediction/main.nf:22:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/chord_prediction/main.nf:87:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_outputs = Channel.empty()
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/cider_calling/main.nf:13:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_inputs        // channel: [mandatory] [ meta ]
      ^^^^^^^^^
  ```

- Warning: `subworkflows/local/cider_calling/main.nf:26:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/cider_calling/main.nf:39:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, bam, bai ->
                               ^^^
  ```

- Warning: `subworkflows/local/cider_calling/main.nf:55:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, bam, bai ->
                               ^^^
  ```

- Warning: `subworkflows/local/cider_calling/main.nf:63:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_cider_inputs = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/cobalt_normalisation/main.nf:24:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/isofox_normalisation/main.nf:23:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/isofox_quantification/main.nf:34:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/isofox_quantification/main.nf:47:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai ->
                                     ^^^^^^^^^
  ```

- Warning: `subworkflows/local/isofox_quantification/main.nf:88:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_outputs = Channel.empty()
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/lilac_calling/main.nf:29:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/lilac_calling/main.nf:47:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai, normal_bam, normal_bai ->
                                     ^^^^^^^^^
  ```

- Warning: `subworkflows/local/lilac_calling/main.nf:47:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai, normal_bam, normal_bai ->
                                                            ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/lilac_calling/main.nf:107:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_outputs = Channel.empty()
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/linx_annotation/main.nf:26:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/linx_annotation/main.nf:99:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, purple_dir ->
                          ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/linx_annotation/main.nf:137:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_somatic_out = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/linx_annotation/main.nf:144:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_germline_out = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/linx_plotting/main.nf:29:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/linx_plotting/main.nf:51:41`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, annotation_dir, amber_dir, cobalt_dir, purple_dir ->
                                          ^^^^^^^^^
  ```

- Warning: `subworkflows/local/linx_plotting/main.nf:51:52`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, annotation_dir, amber_dir, cobalt_dir, purple_dir ->
                                                     ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/linx_plotting/main.nf:51:64`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, annotation_dir, amber_dir, cobalt_dir, purple_dir ->
                                                                 ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/linx_plotting/main.nf:95:38`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, annotation_dir, amber_dir, cobalt_dir, purple_dir, visualiser_dir ->
                                       ^^^^^^^^^
  ```

- Warning: `subworkflows/local/linx_plotting/main.nf:95:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, annotation_dir, amber_dir, cobalt_dir, purple_dir, visualiser_dir ->
                                                  ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/linx_plotting/main.nf:95:61`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, annotation_dir, amber_dir, cobalt_dir, purple_dir, visualiser_dir ->
                                                              ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/linx_plotting/main.nf:115:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_visualiser_dir_out = Channel.empty()
                              ^^^^^^^
  ```

- Warning: `subworkflows/local/pave_annotation/main.nf:34:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/pave_annotation/main.nf:50:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, sage_vcf, sage_tbi ->
                                    ^^^^^^^^
  ```

- Warning: `subworkflows/local/pave_annotation/main.nf:103:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, sage_vcf, sage_tbi ->
                                    ^^^^^^^^
  ```

- Warning: `subworkflows/local/pave_annotation/main.nf:145:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_somatic_out = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/pave_annotation/main.nf:151:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_germline_out = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/pave_pon_creation/main.nf:22:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/peach_calling/main.nf:24:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/peach_calling/main.nf:74:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_outputs = Channel.empty()
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_inputs/main.nf:18:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_inputs = Channel.fromList(
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/redux_processing/main.nf:33:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/redux_processing/main.nf:46:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, bams, bais ->
                                ^^^^
  ```

- Warning: `subworkflows/local/redux_processing/main.nf:61:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, bams, bais ->
                                ^^^^
  ```

- Warning: `subworkflows/local/redux_processing/main.nf:76:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, bams, bais ->
                                ^^^^
  ```

- Warning: `subworkflows/local/redux_processing/main.nf:85:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_redux_inputs = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/redux_processing/main.nf:132:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta_redux, bam, bai, dup_freq_tsv, jitter_tsv, ms_tsv ->
                                ^^^
  ```

- Warning: `subworkflows/local/redux_processing/main.nf:132:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta_redux, bam, bai, dup_freq_tsv, jitter_tsv, ms_tsv ->
                                     ^^^
  ```

- Warning: `subworkflows/local/redux_processing/main.nf:132:41`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta_redux, bam, bai, dup_freq_tsv, jitter_tsv, ms_tsv ->
                                          ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/redux_processing/main.nf:132:55`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta_redux, bam, bai, dup_freq_tsv, jitter_tsv, ms_tsv ->
                                                        ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/redux_processing/main.nf:132:67`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta_redux, bam, bai, dup_freq_tsv, jitter_tsv, ms_tsv ->
                                                                    ^^^^^^
  ```

- Warning: `subworkflows/local/redux_processing/main.nf:142:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_redux_tumor_out = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/redux_processing/main.nf:152:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_redux_normal_out = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/redux_processing/main.nf:162:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_redux_donor_out = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:33:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      segment_mappability          // channel: [mandatory] /path/to/segment_mappability
      ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:43:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:61:13`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              tumor_dup_freq_tsv,  tumor_jitter_tsv,  tumor_ms_tsv,
              ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:62:13`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              normal_dup_freq_tsv, normal_jitter_tsv, normal_ms_tsv,
              ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:63:13`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              donor_dup_freq_tsv,  donor_jitter_tsv,  donor_ms_tsv ->
              ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:76:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              redux_tsv_list = redux_tsv_list.findAll{ it != [] }
                                                       ^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:93:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai, normal_bam, normal_bai, donor_bam, donor_bai, redux_tsvs ->
                                     ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:93:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai, normal_bam, normal_bai, donor_bam, donor_bai, redux_tsvs ->
                                                ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:93:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai, normal_bam, normal_bai, donor_bam, donor_bai, redux_tsvs ->
                                                            ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:93:71`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai, normal_bam, normal_bai, donor_bam, donor_bai, redux_tsvs ->
                                                                        ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:93:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai, normal_bam, normal_bai, donor_bam, donor_bai, redux_tsvs ->
                                                                                   ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:93:93`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai, normal_bam, normal_bai, donor_bam, donor_bai, redux_tsvs ->
                                                                                              ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:106:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai, normal_bam, normal_bai, donor_bam, donor_bai, redux_tsvs ->
                                     ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:106:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai, normal_bam, normal_bai, donor_bam, donor_bai, redux_tsvs ->
                                                            ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:106:71`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai, normal_bam, normal_bai, donor_bam, donor_bai, redux_tsvs ->
                                                                        ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:106:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai, normal_bam, normal_bai, donor_bam, donor_bai, redux_tsvs ->
                                                                                   ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:106:93`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai, normal_bam, normal_bai, donor_bam, donor_bai, redux_tsvs ->
                                                                                              ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:118:68`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, tumor_bam, tumor_bai, normal_bam, normal_bai, donor_bam, donor_bai, redux_tsvs ->
                                                                     ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:118:79`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, tumor_bam, tumor_bai, normal_bam, normal_bai, donor_bam, donor_bai, redux_tsvs ->
                                                                                ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:153:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai, normal_bam, normal_bai, donor_bam, donor_bai, redux_tsvs ->
                                     ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:153:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai, normal_bam, normal_bai, donor_bam, donor_bai, redux_tsvs ->
                                                ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:153:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai, normal_bam, normal_bai, donor_bam, donor_bai, redux_tsvs ->
                                                            ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:153:71`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai, normal_bam, normal_bai, donor_bam, donor_bai, redux_tsvs ->
                                                                        ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:153:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai, normal_bam, normal_bai, donor_bam, donor_bai, redux_tsvs ->
                                                                                   ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:153:93`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_bam, tumor_bai, normal_bam, normal_bai, donor_bam, donor_bai, redux_tsvs ->
                                                                                              ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:206:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_somatic_vcf_out = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:214:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_germline_vcf_out = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:222:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_somatic_dir = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:230:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_germline_dir = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/sigs_fitting/main.nf:22:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/sigs_fitting/main.nf:81:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_outputs = Channel.empty()
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_oncoanalyser_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_oncoanalyser_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `workflows/prepare_reference.nf:24:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/prepare_reference.nf:38:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```
