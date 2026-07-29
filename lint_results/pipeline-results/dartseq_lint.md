# Nextflow lint results

- Generated: 2026-07-29T00:26:28.610273292Z
- Nextflow version: 26.07.0-edge
- Summary: 18 warnings

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

- Warning: `workflows/dartseq.nf:54:68`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(FASTQC.out.zip.collect{it[1]})
                                                                     ^^
  ```

- Warning: `workflows/dartseq.nf:69:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTP.out.html.collect{it[1]})
                                                                         ^^
  ```

- Warning: `workflows/dartseq.nf:70:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTP.out.json.collect{it[1]})
                                                                         ^^
  ```

- Warning: `workflows/dartseq.nf:71:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTP.out.log.collect{it[1]})
                                                                        ^^
  ```

- Warning: `workflows/dartseq.nf:77:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(TRIMGALORE.out.zip.collect{it[1]})
                                                                             ^^
  ```

- Warning: `workflows/dartseq.nf:78:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(TRIMGALORE.out.html.collect{it[1]})
                                                                              ^^
  ```

- Warning: `workflows/dartseq.nf:79:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(TRIMGALORE.out.log.collect{it[1]})
                                                                             ^^
  ```

- Warning: `workflows/dartseq.nf:88:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_fasta = params.fasta ? Channel.value([ [ id: 'fasta' ], file(params.fasta, checkIfExists: true) ]) : channel.empty()
                                    ^^^^^^^
  ```

- Warning: `workflows/dartseq.nf:89:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gtf = params.gtf ? Channel.value([ [ id: 'gtf' ], file(params.gtf, checkIfExists: true) ]) : channel.empty()
                                ^^^^^^^
  ```

- Warning: `workflows/dartseq.nf:100:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ? Channel.value([ [ id: 'star_index' ], file(params.star_index, checkIfExists: true) ])
                    ^^^^^^^
  ```

- Warning: `workflows/dartseq.nf:117:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(STAR_ALIGN.out.log_final.collect{it[1]})
                                                                                       ^^
  ```

- Warning: `workflows/dartseq.nf:129:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ? Channel.value([ [ id: 'hisat2_index' ], file(params.hisat2_index, checkIfExists: true) ])
                    ^^^^^^^
  ```

- Warning: `workflows/dartseq.nf:133:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ? Channel.value([ [ id: 'splicesites' ], file(params.hisat2_splicesites, checkIfExists: true) ])
                    ^^^^^^^
  ```

- Warning: `workflows/dartseq.nf:164:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(HISAT2_ALIGN.out.summary.collect{it[1]})
                                                                                       ^^
  ```

- Warning: `workflows/dartseq.nf:169:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  Channel.value([ [ id: 'no_fasta' ], [], [] ]),
                  ^^^^^^^
  ```

- Warning: `workflows/dartseq.nf:383:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```
