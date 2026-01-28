# Nextflow lint results

- Generated: 2026-01-28T00:18:39.501950776Z
- Nextflow version: 25.12.0-edge
- Summary: 2 errors, 22 warnings

## :x: Errors

- Error: `conf/modules.config:130:22`: `publishDir` is not defined

  ```nextflow
          publishDir = publishDir + [
                       ^^^^^^^^^^
  ```

- Error: `modules/local/multiqc_assemblyscan_plot_data/main.nf:60:40`: `meta` is not defined

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
                                         ^^^^
  ```

## :warning: Warnings

- Warning: `modules/local/multiqc_assemblyscan_plot_data/main.nf:59:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/multiqc_assemblyscan_plot_data/main.nf:60:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/assemblyscan/main.nf:31:9`: Variable was declared but not used

  ```nextflow
      def args        = task.ext.args   ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/last/dotplot/main.nf:45:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/last/lastal/main.nf:94:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/last/lastal/main.nf:96:9`: Variable was declared but not used

  ```nextflow
      def trained_params = param_file ? "-p ${param_file}"  : ''
          ^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/last/lastdb/main.nf:34:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/last/mafconvert/main.nf:89:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/last/split/main.nf:89:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/last/train/main.nf:50:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/pairalign_m2m/main.nf:55:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          training_results_for_multiqc = ALIGNMENT_TRAIN.out.multiqc.collect{ it[1] }
                                                                              ^^
  ```

- Warning: `subworkflows/local/pairalign_m2m/main.nf:152:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      multiqc = Channel.empty()
                ^^^^^^^
  ```

- Warning: `subworkflows/local/pairalign_m2m/main.nf:154:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .mix(ALIGNMENT_SPLIT_O2O.out.multiqc.collect{ it[1]} )
                                                        ^^
  ```

- Warning: `subworkflows/local/pairalign_m2o/main.nf:49:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          training_results_for_multiqc = ALIGNMENT_TRAIN.out.multiqc.collect{ it[1] }
                                                                              ^^
  ```

- Warning: `subworkflows/local/pairalign_m2o/main.nf:105:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      multiqc = Channel.empty()
                ^^^^^^^
  ```

- Warning: `subworkflows/local/pairalign_m2o/main.nf:107:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .mix(ALIGNMENT_SPLIT_O2O.out.multiqc.collect{ it[1]} )
                                                        ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pairgenomealign_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pairgenomealign_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `workflows/pairgenomealign.nf:41:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_targetgenome.map { meta, file -> [ [id:'targetGenome'] , file ] }
                                ^^^^
  ```

- Warning: `workflows/pairgenomealign.nf:53:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
            .map { sorted_list -> sorted_list.collect { it[1] } }
                                                        ^^
  ```

- Warning: `workflows/pairgenomealign.nf:106:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              pairalign_out.o2o.combine(Channel.fromList(export_formats)),
                                        ^^^^^^^
  ```

- Warning: `workflows/pairgenomealign.nf:116:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```
