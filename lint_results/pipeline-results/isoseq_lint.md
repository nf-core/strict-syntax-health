# Nextflow lint results

- Generated: 2026-07-03T00:34:05.694302588Z
- Nextflow version: 26.06.0-edge
- Summary: 19 warnings

## :warning: Warnings

- Warning: `main.nf:61:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = ISOSEQ.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/gstama/filelist/main.nf:20:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/chunker/main.nf:39:16`: Variable was declared but not used

  ```nextflow
          .set { fastas }
                 ^^^^^^
  ```

- Warning: `subworkflows/local/chunker/main.nf:42:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      fastas
      ^^^^^^
  ```

- Warning: `subworkflows/local/set_chunk_num_channel/main.nf:15:16`: Variable was declared but not used

  ```nextflow
          .set { chunk_num }
                 ^^^^^^^^^
  ```

- Warning: `subworkflows/local/set_chunk_num_channel/main.nf:18:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      chunk_num
      ^^^^^^^^^
  ```

- Warning: `subworkflows/local/set_value_channel/main.nf:15:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { it[1] }
                     ^^
  ```

- Warning: `subworkflows/local/set_value_channel/main.nf:26:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      data // channel: [ file(infile) ]
      ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_isoseq_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

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

- Warning: `workflows/isoseq.nf:151:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { meta, files -> [ meta, [files].flatten().find { !it.name.endsWith('_tails.fa.gz') } ] }
                                                                  ^^
  ```

- Warning: `workflows/isoseq.nf:215:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      GSTAMA_MERGE(ch_tmerge_in.map { [ it[0], it[1] ] }, ch_tmerge_in.map { it[2] }) // Merge all bed files from one sample into a uniq bed file
                                        ^^
  ```

- Warning: `workflows/isoseq.nf:215:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      GSTAMA_MERGE(ch_tmerge_in.map { [ it[0], it[1] ] }, ch_tmerge_in.map { it[2] }) // Merge all bed files from one sample into a uniq bed file
                                               ^^
  ```

- Warning: `workflows/isoseq.nf:215:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      GSTAMA_MERGE(ch_tmerge_in.map { [ it[0], it[1] ] }, ch_tmerge_in.map { it[2] }) // Merge all bed files from one sample into a uniq bed file
                                                                             ^^
  ```

- Warning: `workflows/isoseq.nf:285:75`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(PBCCS.out.report_json.collect{it[1]}.ifEmpty([]))
                                                                            ^^
  ```

- Warning: `workflows/isoseq.nf:286:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(LIMA.out.summary.collect{it[1]}.ifEmpty([]))
                                                                       ^^
  ```

- Warning: `workflows/isoseq.nf:287:69`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(LIMA.out.counts.collect{it[1]}.ifEmpty([]))
                                                                      ^^
  ```
