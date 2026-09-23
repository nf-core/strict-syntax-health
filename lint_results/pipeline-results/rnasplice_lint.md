# Nextflow lint results

- Generated: 2026-09-23T00:25:04.822698475Z
- Nextflow version: 26.08.0-edge
- Summary: 13 warnings

## :warning: Warnings

- Warning: `conf/modules.config:333:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:342:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:351:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:360:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:382:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `modules/local/mergeevents/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/misopysettings/main.nf:26:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/tximeta/tximport/main.nf:50:9`: Variable was declared but not used

  ```nextflow
      def prefix            = task.ext.prefix ?: meta.id
          ^^^^^^
  ```

- Warning: `modules/local/tximeta/tximport/main.nf:51:9`: Variable was declared but not used

  ```nextflow
      def ignore_tx_version = task.ext.args ?: 'false'
          ^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/misopy/index/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_rnasplice_pipeline/main.nf:531:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              if (it.size() > 1) {
                  ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_rnasplice_pipeline/main.nf:546:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              if (it.size() > 1) {
                  ^^
  ```

- Warning: `workflows/rnasplice.nf:179:9`: Variable was declared but not used

  ```nextflow
          ch_transcriptome_bam_index = BAM_SORT_STATS_SAMTOOLS.out.index
          ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```
