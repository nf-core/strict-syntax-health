# Nextflow lint results

- Generated: 2026-10-14T00:19:25.870065258Z
- Nextflow version: 26.10.0
- Summary: 38 warnings

## :warning: Warnings

- Warning: `modules/local/bullseye/acfilter/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/bullseye/findeditsites/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/bullseye/gathersites/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/bullseye/gtf2genepred/main.nf:14:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/bullseye/parsebam/main.nf:16:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/bullseye/quantifysites/main.nf:16:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/bullseye/racfilter/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/bullseye/rglm/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/bullseye/summarizesites/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/fastp/main.nf:25:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/fastqc/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/hisat2/align/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/hisat2/build/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/hisat2/extractsplicesites/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/multiqc/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/index/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/sort/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/star/align/main.nf:38:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/star/genomegenerate/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/trimgalore/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

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

- Warning: `workflows/dartseq.nf:135:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ? Channel.value([ [ id: 'hisat2_index' ], file(params.hisat2_index, checkIfExists: true) ])
                    ^^^^^^^
  ```

- Warning: `workflows/dartseq.nf:139:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ? Channel.value([ [ id: 'splicesites' ], file(params.hisat2_splicesites, checkIfExists: true) ])
                    ^^^^^^^
  ```

- Warning: `workflows/dartseq.nf:170:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(HISAT2_ALIGN.out.summary.collect{it[1]})
                                                                                       ^^
  ```

- Warning: `workflows/dartseq.nf:175:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  Channel.value([ [ id: 'no_fasta' ], [], [] ]),
                  ^^^^^^^
  ```

- Warning: `workflows/dartseq.nf:417:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```
