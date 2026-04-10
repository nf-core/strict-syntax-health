# Nextflow lint results

- Generated: 2026-04-10T00:23:16.428969774Z
- Nextflow version: 26.03.2-edge
- Summary: 17 warnings

## :warning: Warnings

- Warning: `modules/local/hmmer/hmmextract/main.nf:50:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:59:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:61:9`: Variable was declared but not used

  ```nextflow
      def paired       = meta.single_end ? "" : "--paired"
          ^^^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:64:9`: Variable was declared but not used

  ```nextflow
      def readclassification_option = save_reads_assignment ? "--output ${prefix}.kraken2.classifiedreads.txt" : "--output /dev/null"
          ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:65:9`: Variable was declared but not used

  ```nextflow
      def compress_reads_command = save_output_fastqs ? "pigz -p $task.cpus *.fastq" : ""
          ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/pigz/uncompress/main.nf:39:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/vsearch/cluster/main.nf:78:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_ampliseq_pipeline/main.nf:374:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          if (sectionValue instanceof Map && sectionValue.any { it.value instanceof Map && it.value.containsKey('file') }) {
                                                                ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_ampliseq_pipeline/main.nf:374:90`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          if (sectionValue instanceof Map && sectionValue.any { it.value instanceof Map && it.value.containsKey('file') }) {
                                                                                           ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_ampliseq_pipeline/main.nf:408:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      occurrences.collect { "${it.section}['${it.key}']" }.join(", ")
                                               ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_ampliseq_pipeline/main.nf:408:61`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      occurrences.collect { "${it.section}['${it.key}']" }.join(", ")
                                                              ^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```

- Warning: `workflows/ampliseq.nf:190:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_pplace_sheet = Channel.fromPath(params.pplace_sheet)
                            ^^^^^^^
  ```

- Warning: `workflows/ampliseq.nf:796:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it.data.extract_hmm }
                    ^^
  ```

- Warning: `workflows/ampliseq.nf:797:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [ it.meta, it.data.hmm, it.data.extract_hmm ] }
                   ^^
  ```

- Warning: `workflows/ampliseq.nf:797:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [ it.meta, it.data.hmm, it.data.extract_hmm ] }
                            ^^
  ```

- Warning: `workflows/ampliseq.nf:797:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [ it.meta, it.data.hmm, it.data.extract_hmm ] }
                                         ^^
  ```
