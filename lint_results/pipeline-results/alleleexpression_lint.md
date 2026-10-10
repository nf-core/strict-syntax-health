# Nextflow lint results

- Generated: 2026-10-10T00:21:00.984879178Z
- Nextflow version: 26.09.2-edge
- Summary: 20 warnings

## :warning: Warnings

- Warning: `modules/local/star_align_wasp/main.nf:47:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      meta.single_end ? [reads].flatten().each{reads1 << it} : reads.eachWithIndex{ v, ix -> ( ix & 1 ? reads2 : reads1) << v }
                                                         ^^
  ```

- Warning: `modules/local/star_align_wasp/main.nf:61:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      if (reads1.any { it.toString().endsWith('.gz') } || reads2.any { it.toString().endsWith('.gz') }) {
                       ^^
  ```

- Warning: `modules/local/star_align_wasp/main.nf:61:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      if (reads1.any { it.toString().endsWith('.gz') } || reads2.any { it.toString().endsWith('.gz') }) {
                                                                       ^^
  ```

- Warning: `modules/nf-core/bcftools/index/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/bcftools/index/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/star/align/main.nf:46:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      meta.single_end ? [reads].flatten().each{reads1 << it} : reads.eachWithIndex{ v, ix -> ( ix & 1 ? reads2 : reads1) << v }
                                                         ^^
  ```

- Warning: `workflows/alleleexpression.nf:38:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/alleleexpression.nf:77:14`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gtf = Channel.fromPath(params.gtf, checkIfExists: true)
               ^^^^^^^
  ```

- Warning: `workflows/alleleexpression.nf:83:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_star_index = Channel.fromPath(params.star_index, checkIfExists: true)
                          ^^^^^^^
  ```

- Warning: `workflows/alleleexpression.nf:87:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_fasta = Channel.fromPath(params.fasta, checkIfExists: true)
                     ^^^^^^^
  ```

- Warning: `workflows/alleleexpression.nf:126:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.value([['id': 'dummy'], []])
          ^^^^^^^
  ```

- Warning: `workflows/alleleexpression.nf:160:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.fromPath(params.beagle_ref).first() :
          ^^^^^^^
  ```

- Warning: `workflows/alleleexpression.nf:161:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.empty()
          ^^^^^^^
  ```

- Warning: `workflows/alleleexpression.nf:163:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.fromPath(params.beagle_map).first() :
          ^^^^^^^
  ```

- Warning: `workflows/alleleexpression.nf:164:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.empty()
          ^^^^^^^
  ```

- Warning: `workflows/alleleexpression.nf:195:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gene_features = Channel.fromPath(params.gene_features).first()
                         ^^^^^^^
  ```

- Warning: `workflows/alleleexpression.nf:248:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `workflows/alleleexpression.nf:249:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .mix(FASTQC.out.zip.collect { it[1] })
                                        ^^
  ```

- Warning: `workflows/alleleexpression.nf:250:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .mix(STAR_ALIGN_WASP.out.log_final.collect { it[1] })
                                                       ^^
  ```

- Warning: `workflows/alleleexpression.nf:251:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .mix(UMITOOLS_DEDUP.out.log.collect { it[1] })
                                                ^^
  ```
