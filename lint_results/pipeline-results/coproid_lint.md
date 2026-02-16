# Nextflow lint results

- Generated: 2026-02-16T00:19:47.188987641Z
- Nextflow version: 26.01.1-edge
- Summary: 12 errors, 46 warnings

## :x: Errors

- Error: `modules/nf-core/quartonotebook/parametrize.nf:1:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import org.yaml.snakeyaml.Yaml
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `modules/nf-core/quartonotebook/parametrize.nf:2:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import org.yaml.snakeyaml.DumperOptions
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `modules/nf-core/quartonotebook/parametrize.nf:21:29`: `DumperOptions` is not defined

  ```nextflow
      DumperOptions options = new DumperOptions();
                              ^^^^^^^^^^^^^^^^^^^
  ```

- Error: `modules/nf-core/quartonotebook/parametrize.nf:22:33`: `DumperOptions` is not defined

  ```nextflow
      options.setDefaultFlowStyle(DumperOptions.FlowStyle.BLOCK);
                                  ^^^^^^^^^^^^^
  ```

- Error: `modules/nf-core/quartonotebook/parametrize.nf:23:16`: `Yaml` is not defined

  ```nextflow
      def yaml = new Yaml(options)
                 ^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/kraken2_classification/main.nf:25:20`: `kraken2_db` is already declared

  ```nextflow
              .map { kraken2_db ->
                     ^^^^^^^^^^
  ```

- Error: `subworkflows/local/prepare_genome_indices/main.nf:48:49`: `igenome` is not defined

  ```nextflow
          genome_meta = [meta, file(params.genomes[ igenome ][ fasta ]), path(params.genomes[ igenome ][ bowtie2 ])]
                                                  ^^^^^^^^^^^
  ```

- Error: `subworkflows/local/prepare_genome_indices/main.nf:48:60`: `fasta` is not defined

  ```nextflow
          genome_meta = [meta, file(params.genomes[ igenome ][ fasta ]), path(params.genomes[ igenome ][ bowtie2 ])]
                                                             ^^^^^^^^^
  ```

- Error: `subworkflows/local/prepare_genome_indices/main.nf:48:72`: `path` is not defined

  ```nextflow
          genome_meta = [meta, file(params.genomes[ igenome ][ fasta ]), path(params.genomes[ igenome ][ bowtie2 ])]
                                                                         ^^^^
  ```

- Error: `subworkflows/local/prepare_genome_indices/main.nf:48:91`: `igenome` is not defined

  ```nextflow
          genome_meta = [meta, file(params.genomes[ igenome ][ fasta ]), path(params.genomes[ igenome ][ bowtie2 ])]
                                                                                            ^^^^^^^^^^^
  ```

- Error: `subworkflows/local/prepare_genome_indices/main.nf:48:102`: `bowtie2` is not defined

  ```nextflow
          genome_meta = [meta, file(params.genomes[ igenome ][ fasta ]), path(params.genomes[ igenome ][ bowtie2 ])]
                                                                                                       ^^^^^^^^^^^
  ```

- Error: `subworkflows/local/quarto_reporting/main.nf:26:9`: `coproid_notebook` is already declared

  ```nextflow
          coproid_notebook ->
          ^^^^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `modules/local/create_acc2tax/main.nf:18:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ""
          ^^^^
  ```

- Warning: `modules/local/damageprofiler/merge/main.nf:17:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args   ?: ''
          ^^^^
  ```

- Warning: `modules/local/kraken/merge/main.nf:18:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args   ?: ''
          ^^^^
  ```

- Warning: `modules/local/kraken/parse/main.nf:19:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args   ?: ''
          ^^^^
  ```

- Warning: `modules/local/pydamage/merge/main.nf:17:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args   ?: ''
          ^^^^
  ```

- Warning: `modules/local/sam2lca/merge/main.nf:18:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args   ?: ''
          ^^^^
  ```

- Warning: `modules/local/sam2lca/prep_db/main.nf:19:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ""
          ^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:60:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:62:9`: Variable was declared but not used

  ```nextflow
      def paired       = meta.single_end ? "" : "--paired"
          ^^^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:65:9`: Variable was declared but not used

  ```nextflow
      def readclassification_option = save_reads_assignment ? "--output ${prefix}.kraken2.classifiedreads.txt" : "--output /dev/null"
          ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:66:9`: Variable was declared but not used

  ```nextflow
      def compress_reads_command = save_output_fastqs ? "pigz -p $task.cpus *.fastq" : ""
          ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/quartonotebook/main.nf:102:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/sourcepredict/main.nf:47:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/align_index/main.nf:9:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_versions = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/kraken2_classification/main.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/kraken2_classification/main.nf:23:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel
          ^^^^^^^
  ```

- Warning: `subworkflows/local/kraken2_classification/main.nf:82:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          sqlite = XZ_DECOMPRESS.out.file.map { it[1] }
                                                ^^
  ```

- Warning: `subworkflows/local/merge_sort_index_samtools/main.nf:10:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome_indices/main.nf:9:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome_indices/main.nf:12:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { create_genome_channel(it) }
                                       ^^
  ```

- Warning: `subworkflows/local/prepare_genome_indices/main.nf:17:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              index_avail: it.size() > 2
                           ^^
  ```

- Warning: `subworkflows/local/prepare_genome_indices/main.nf:18:29`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_index_avail: it.size() == 2
                              ^^
  ```

- Warning: `subworkflows/local/quarto_reporting/main.nf:14:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/quarto_reporting/main.nf:20:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      extensions = Channel.fromPath("${projectDir}/assets/_extensions").collect()
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/quarto_reporting/main.nf:23:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `subworkflows/local/sam2lca_db/main.nf:15:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_versions = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_coproid_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_coproid_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_coproid_pipeline/main.nf:39:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      genome_sheet //  string: Path to reference genomesheet
      ^^^^^^^^^^^^
  ```

- Warning: `workflows/coproid.nf:71:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(FASTQC.out.zip.collect { it[1] })
                                                                       ^^
  ```

- Warning: `workflows/coproid.nf:83:5`: Variable was declared but not used

  ```nextflow
      ch_trimmed = FASTP.out.reads
      ^^^^^^^^^^
  ```

- Warning: `workflows/coproid.nf:84:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(FASTP.out.json.collect { it[1] })
                                                                       ^^
  ```

- Warning: `workflows/coproid.nf:115:85`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(ALIGN_INDEX.out.multiqc_files.collect { it[1] })
                                                                                      ^^
  ```

- Warning: `workflows/coproid.nf:124:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(DAMAGEPROFILER.out.results.collect { it[1] })
                                                                                   ^^
  ```

- Warning: `workflows/coproid.nf:127:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .collect { it[1] }
                     ^^
  ```

- Warning: `workflows/coproid.nf:150:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .collect { it[1] }
                     ^^
  ```

- Warning: `workflows/coproid.nf:163:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, bam, bai ->
                            ^^^
  ```

- Warning: `workflows/coproid.nf:178:60`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              PREPARE_GENOMES.out.genomes.map { meta, fasta, index ->
                                                             ^^^^^
  ```

- Warning: `workflows/coproid.nf:190:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_sam2lca_db = Channel.fromPath(params.sam2lca_db).first()
                          ^^^^^^^
  ```

- Warning: `workflows/coproid.nf:202:5`: Variable was declared but not used

  ```nextflow
      ch_sam2lca = SAM2LCA_ANALYZE.out.csv
      ^^^^^^^^^^
  ```

- Warning: `workflows/coproid.nf:206:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .collect { it[1] }
                     ^^
  ```

- Warning: `workflows/coproid.nf:221:96`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(KRAKEN2_CLASSIFICATION.out.kraken_report.collect { it[1] })
                                                                                                 ^^
  ```

- Warning: `workflows/coproid.nf:227:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel
                           ^^^^^^^
  ```

- Warning: `workflows/coproid.nf:258:64`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              KRAKEN2_CLASSIFICATION.out.sp_report.collectFile { it[1] },
                                                                 ^^
  ```

- Warning: `workflows/coproid.nf:259:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              KRAKEN2_CLASSIFICATION.out.sp_embedding.collectFile { it[1] },
                                                                    ^^
  ```

- Warning: `workflows/coproid.nf:262:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              Channel.fromPath(params.genome_sheet),
              ^^^^^^^
  ```
