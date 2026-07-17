# Nextflow lint results

- Generated: 2026-07-17T00:29:08.458470280Z
- Nextflow version: 26.07.0-edge
- Summary: 5 warnings

## :warning: Warnings

- Warning: `modules/local/comparechecksum/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/comparechecksum/main.nf:27:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `workflows/datasync.nf:81:78`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(COMPARECHECKSUM.out.report.map { meta, report -> report })
                                                                               ^^^^
  ```

- Warning: `workflows/datasync.nf:82:86`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(COMPARECHECKSUM.out.summary_report.map { meta, summary -> summary })
                                                                                       ^^^^
  ```

- Warning: `workflows/datasync.nf:124:45`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(Channel.fromPath(params.input).collectFile(name: 'samplesheet.csv'))
                                              ^^^^^^^
  ```
