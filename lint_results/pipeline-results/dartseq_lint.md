# Nextflow lint results

- Generated: 2026-05-21T00:40:16.677281966Z
- Nextflow version: 26.04.1
- Summary: 19 warnings

## :warning: Warnings

- Warning: `subworkflows/local/utils_nfcore_dartseq_pipeline/main.nf:31:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_dartseq_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```

- Warning: `workflows/dartseq.nf:52:68`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(FASTQC.out.zip.collect{it[1]})
                                                                     ^^
  ```

- Warning: `workflows/dartseq.nf:67:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTP.out.html.collect{it[1]})
                                                                         ^^
  ```

- Warning: `workflows/dartseq.nf:68:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTP.out.json.collect{it[1]})
                                                                         ^^
  ```

- Warning: `workflows/dartseq.nf:69:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTP.out.log.collect{it[1]})
                                                                        ^^
  ```

- Warning: `workflows/dartseq.nf:75:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(TRIMGALORE.out.zip.collect{it[1]})
                                                                             ^^
  ```

- Warning: `workflows/dartseq.nf:76:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(TRIMGALORE.out.html.collect{it[1]})
                                                                              ^^
  ```

- Warning: `workflows/dartseq.nf:77:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(TRIMGALORE.out.log.collect{it[1]})
                                                                             ^^
  ```

- Warning: `workflows/dartseq.nf:86:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_fasta = params.fasta ? Channel.value([ [ id: 'fasta' ], file(params.fasta, checkIfExists: true) ]) : channel.empty()
                                    ^^^^^^^
  ```

- Warning: `workflows/dartseq.nf:87:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gtf = params.gtf ? Channel.value([ [ id: 'gtf' ], file(params.gtf, checkIfExists: true) ]) : channel.empty()
                                ^^^^^^^
  ```

- Warning: `workflows/dartseq.nf:98:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ? Channel.value([ [ id: 'star_index' ], file(params.star_index, checkIfExists: true) ])
                    ^^^^^^^
  ```

- Warning: `workflows/dartseq.nf:115:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(STAR_ALIGN.out.log_final.collect{it[1]})
                                                                                       ^^
  ```

- Warning: `workflows/dartseq.nf:127:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ? Channel.value([ [ id: 'hisat2_index' ], file(params.hisat2_index, checkIfExists: true) ])
                    ^^^^^^^
  ```

- Warning: `workflows/dartseq.nf:131:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ? Channel.value([ [ id: 'splicesites' ], file(params.hisat2_splicesites, checkIfExists: true) ])
                    ^^^^^^^
  ```

- Warning: `workflows/dartseq.nf:162:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(HISAT2_ALIGN.out.summary.collect{it[1]})
                                                                                       ^^
  ```

- Warning: `workflows/dartseq.nf:167:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  Channel.value([ [ id: 'no_fasta' ], [], [] ]),
                  ^^^^^^^
  ```

- Warning: `workflows/dartseq.nf:373:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```
