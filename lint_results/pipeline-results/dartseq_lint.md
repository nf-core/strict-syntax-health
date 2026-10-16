# Nextflow lint results

- Generated: 2026-10-16T00:18:13.500249893Z
- Nextflow version: 26.10.1
- Summary: 34 warnings

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

- Warning: `modules/nf-core/multiqc/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

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

- Warning: `workflows/dartseq.nf:71:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTP.out.html.collect{it[1]})
                                                                         ^^
  ```

- Warning: `workflows/dartseq.nf:72:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTP.out.json.collect{it[1]})
                                                                         ^^
  ```

- Warning: `workflows/dartseq.nf:73:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTP.out.log.collect{it[1]})
                                                                        ^^
  ```

- Warning: `workflows/dartseq.nf:79:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(TRIMGALORE.out.zip.collect{it[1]})
                                                                             ^^
  ```

- Warning: `workflows/dartseq.nf:80:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(TRIMGALORE.out.html.collect{it[1]})
                                                                              ^^
  ```

- Warning: `workflows/dartseq.nf:81:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(TRIMGALORE.out.log.collect{it[1]})
                                                                             ^^
  ```

- Warning: `workflows/dartseq.nf:90:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_fasta = params.fasta ? Channel.value([ [ id: 'fasta' ], file(params.fasta, checkIfExists: true) ]) : channel.empty()
                                    ^^^^^^^
  ```

- Warning: `workflows/dartseq.nf:91:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gtf = params.gtf ? Channel.value([ [ id: 'gtf' ], file(params.gtf, checkIfExists: true) ]) : channel.empty()
                                ^^^^^^^
  ```

- Warning: `workflows/dartseq.nf:102:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ? Channel.value([ [ id: 'star_index' ], file(params.star_index, checkIfExists: true) ])
                    ^^^^^^^
  ```

- Warning: `workflows/dartseq.nf:119:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(STAR_ALIGN.out.log_final.collect{it[1]})
                                                                                       ^^
  ```

- Warning: `workflows/dartseq.nf:137:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ? Channel.value([ [ id: 'hisat2_index' ], file(params.hisat2_index, checkIfExists: true) ])
                    ^^^^^^^
  ```

- Warning: `workflows/dartseq.nf:141:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  ? Channel.value([ [ id: 'splicesites' ], file(params.hisat2_splicesites, checkIfExists: true) ])
                    ^^^^^^^
  ```

- Warning: `workflows/dartseq.nf:172:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(HISAT2_ALIGN.out.summary.collect{it[1]})
                                                                                       ^^
  ```

- Warning: `workflows/dartseq.nf:177:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  Channel.value([ [ id: 'no_fasta' ], [], [] ]),
                  ^^^^^^^
  ```
