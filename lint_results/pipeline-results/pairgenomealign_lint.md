# Nextflow lint results

- Generated: 2026-11-03T00:13:55.095361437Z
- Nextflow version: 26.10.5
- Summary: 27 warnings

## :warning: Warnings

- Warning: `modules/local/multiqc_assemblyscan_plot_data/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/multiqc_thumbs_html/main.nf:16:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/assemblyscan/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/htslib/bgziptabix/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/last/dotplot/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/last/lastal/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/last/lastdb/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/last/mafconvert/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/last/split/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/last/train/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/multiqc/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/dict/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/faidx/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/merge/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/seqtk/cutn/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
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

- Warning: `workflows/pairgenomealign.nf:121:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              o2o_alignments.map {it + "cram"},
                                  ^^
  ```

- Warning: `workflows/pairgenomealign.nf:127:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, cram -> tuple(params.targetName, cram) }
                     ^^^^
  ```

- Warning: `workflows/pairgenomealign.nf:148:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .map { meta, file -> file }
                         ^^^^
  ```
