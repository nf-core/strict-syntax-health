# Nextflow lint results

- Generated: 2026-06-03T00:51:44.633746110Z
- Nextflow version: 26.04.3
- Summary: 26 warnings

## :warning: Warnings

- Warning: `main.nf:62:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = PAIRGENOMEALIGN.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
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

- Warning: `subworkflows/local/utils_nfcore_pairgenomealign_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/nf-core/fasta_bgzip_index_dict_samtools/main.nf:35:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      fasta_fai_gzi_dict = ch_joined             // channel: [ val(meta),  fasta.gz, fai, gzi, sizes, dict ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
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

- Warning: `workflows/pairgenomealign.nf:50:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_targetgenome.map { meta, file -> [ [id:'targetGenome'] , file ] }
                                ^^^^
  ```

- Warning: `workflows/pairgenomealign.nf:62:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
            .map { sorted_list -> sorted_list.collect { it[1] } }
                                                        ^^
  ```

- Warning: `workflows/pairgenomealign.nf:113:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              pairalign_out.o2o.combine(Channel.fromList(export_formats)),
                                        ^^^^^^^
  ```

- Warning: `workflows/pairgenomealign.nf:129:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              o2o_alignments.map {it + "cram"},
                                  ^^
  ```

- Warning: `workflows/pairgenomealign.nf:138:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, cram -> tuple(params.targetName, cram) }
                     ^^^^
  ```

- Warning: `workflows/pairgenomealign.nf:159:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .map { meta, file -> file }
                         ^^^^
  ```
