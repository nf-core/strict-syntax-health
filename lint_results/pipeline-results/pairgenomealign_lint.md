# Nextflow lint results

- Generated: 2026-07-14T00:26:42.222777629Z
- Nextflow version: 26.06.0-edge
- Summary: 17 warnings

## :warning: Warnings

- Warning: `main.nf:60:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = PAIRGENOMEALIGN.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/pairalign_m2m/main.nf:55:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          training_results_for_multiqc = ALIGNMENT_TRAIN.out.multiqc.collect{ it[1] }
                                                                              ^^
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

- Warning: `workflows/pairgenomealign.nf:45:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_targetgenome = ch_samplesheet.map { meta, query, target -> [ [id:meta.targetName], target ] }.first()
                                                   ^^^^^
  ```

- Warning: `workflows/pairgenomealign.nf:46:57`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_querygenome  = ch_samplesheet.map { meta, query, target -> [ meta, query ] }
                                                          ^^^^^^
  ```

- Warning: `workflows/pairgenomealign.nf:50:81`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def needs_genome = ['cram','bam','bcf','gff'].any { export_formats.contains(it) }
                                                                                  ^^
  ```

- Warning: `workflows/pairgenomealign.nf:71:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
            .map { sorted_list -> sorted_list.collect { it[1] } }
                                                        ^^
  ```

- Warning: `workflows/pairgenomealign.nf:120:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              o2o_alignments.map {it + "cram"},
                                  ^^
  ```

- Warning: `workflows/pairgenomealign.nf:126:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, cram -> tuple(params.targetName, cram) }
                     ^^^^
  ```

- Warning: `workflows/pairgenomealign.nf:147:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .map { meta, file -> file }
                         ^^^^
  ```
