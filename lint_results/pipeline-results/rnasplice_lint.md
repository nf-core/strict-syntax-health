# Nextflow lint results

- Generated: 2026-07-18T00:27:51.072295182Z
- Nextflow version: 26.07.0-edge
- Summary: 21 warnings

## :warning: Warnings

- Warning: `conf/modules.config:305:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:314:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:323:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:332:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:354:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `modules/nf-core/misopy/index/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `subworkflows/local/dexseq_deu/main.nf:55:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          DEXSEQ_COUNT.out.dexseq_clean_txt.map{ it[1] }.collect(),
                                                 ^^
  ```

- Warning: `subworkflows/local/dexseq_deu/main.nf:64:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      dexseq_clean_txt        = DEXSEQ_COUNT.out.dexseq_clean_txt.map{ it[1] }.collect()
                                                                       ^^
  ```

- Warning: `subworkflows/local/tx2gene_tximport/main.nf:29:14`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          tar: it[0].tgz == true
               ^^
  ```

- Warning: `subworkflows/local/tx2gene_tximport/main.nf:30:14`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          dir: it[0].tgz == false
               ^^
  ```

- Warning: `subworkflows/local/tx2gene_tximport/main.nf:44:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      TXIMPORT ( salmon_results.collect{it[1]}, tx2gene )
                                        ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_rnasplice_pipeline/main.nf:411:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, fastq -> meta.single_end }
                       ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_rnasplice_pipeline/main.nf:415:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              if (it.size() > 1) {
                  ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_rnasplice_pipeline/main.nf:426:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, fastq -> meta.strandedness }
                       ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_rnasplice_pipeline/main.nf:430:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              if (it.size() > 1) {
                  ^^
  ```

- Warning: `workflows/rnasplice.nf:71:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      multiqc_config // parameter value pass-through
      ^^^^^^^^^^^^^^
  ```

- Warning: `workflows/rnasplice.nf:72:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      multiqc_logo // parameter value pass-through
      ^^^^^^^^^^^^
  ```

- Warning: `workflows/rnasplice.nf:73:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      multiqc_methods_description // parameter value pass-through
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/rnasplice.nf:135:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .flatMap { it }
                     ^^
  ```

- Warning: `workflows/rnasplice.nf:136:16`: Variable was declared but not used

  ```nextflow
          .set { ch_contrasts }
                 ^^^^^^^^^^^^
  ```

- Warning: `workflows/rnasplice.nf:227:9`: Variable was declared but not used

  ```nextflow
          ch_transcriptome_bam_index = BAM_SORT_STATS_SAMTOOLS.out.index
          ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```
