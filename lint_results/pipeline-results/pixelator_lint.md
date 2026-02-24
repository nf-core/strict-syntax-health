# Nextflow lint results

- Generated: 2026-02-24T00:23:05.355143633Z
- Nextflow version: 26.01.1-edge
- Summary: 10 errors, 38 warnings

## :x: Errors

- Error: `conf/modules.config:36:9`: If statements cannot be mixed with config statements

  ```nextflow
          if (params.pixelator_container) {
          ^
  ```

- Error: `nextflow.config:130:1`: Variable declarations cannot be mixed with config statements

  ```nextflow
  def container_env_options = [
  ^
  ```

- Error: `nextflow.config:178:32`: `container_env_options` is not defined

  ```nextflow
          env                  = container_env_options
                                 ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `nextflow.config:203:34`: `container_env_options` is not defined

  ```nextflow
          env                    = container_env_options
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `nextflow.config:214:32`: `container_env_options` is not defined

  ```nextflow
          env                  = container_env_options
                                 ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `nextflow.config:224:32`: `container_env_options` is not defined

  ```nextflow
          env                  = container_env_options
                                 ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `nextflow.config:234:32`: `container_env_options` is not defined

  ```nextflow
          env                  = container_env_options
                                 ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `nextflow.config:245:32`: `container_env_options` is not defined

  ```nextflow
          env                  = container_env_options
                                 ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/pixelator.nf:12:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  if (params.input) {
  ^
  ```

- Error: `workflows/pixelator.nf:107:22`: `_` is not allowed as an identifier because it is reserved for future use

  ```nextflow
          .map { meta, _ -> [meta.id, meta] }
                       ^
  ```

## :warning: Warnings

- Warning: `conf/modules.pna.config:35:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_pna_amplicon_reads || params.save_all ? it : null },
                                                                                ^^
  ```

- Warning: `conf/modules.pna.config:46:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_json || params.save_all ? it : null },
                                                                  ^^
  ```

- Warning: `conf/modules.pna.config:65:78`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_pna_demux_parquet || params.save_all ? it : null },
                                                                               ^^
  ```

- Warning: `conf/modules.pna.config:71:83`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_pna_demux_passed_reads || params.save_all ? it : null },
                                                                                    ^^
  ```

- Warning: `conf/modules.pna.config:77:83`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_pna_demux_failed_reads || params.save_all ? it : null },
                                                                                    ^^
  ```

- Warning: `conf/modules.pna.config:88:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_json || params.save_all ? it : null },
                                                                  ^^
  ```

- Warning: `conf/modules.pna.config:105:80`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_pna_collapsed_reads || params.save_all ? it : null },
                                                                                 ^^
  ```

- Warning: `conf/modules.pna.config:116:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_json || params.save_all ? it : null },
                                                                  ^^
  ```

- Warning: `conf/modules.pna.config:144:80`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_pna_graph_pixelfile || params.save_all ? it : null },
                                                                                 ^^
  ```

- Warning: `conf/modules.pna.config:155:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_json || params.save_all ? it : null },
                                                                  ^^
  ```

- Warning: `conf/modules.pna.config:176:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          return it
                                 ^^
  ```

- Warning: `conf/modules.pna.config:190:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_json ? it : null },
                                               ^^
  ```

- Warning: `conf/modules.pna.config:215:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          return it
                                 ^^
  ```

- Warning: `conf/modules.pna.config:229:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_json || params.save_all ? it : null },
                                                                  ^^
  ```

- Warning: `conf/modules.pna.config:251:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      new File(it).name
                               ^^
  ```

- Warning: `conf/modules.pna.config:263:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_json || params.save_all ? it : null },
                                                                  ^^
  ```

- Warning: `modules/local/pixelator/single-cell-pna/amplicon/main.nf:28:9`: Variable was declared but not used

  ```nextflow
      def r = reads
          ^
  ```

- Warning: `modules/local/pixelator/single-cell-pna/amplicon/main.nf:37:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def renamed_reads = old_new_pairs.collect { old_name, new_name -> new_name }.join(' ')
                                                  ^^^^^^^^
  ```

- Warning: `modules/nf-core/cat/fastq/main.nf:22:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def readList = reads instanceof List ? reads.collect { it.toString() } : [reads.toString()]
                                                             ^^
  ```

- Warning: `modules/nf-core/cat/fastq/main.nf:48:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def readList = reads instanceof List ? reads.collect { it.toString() } : [reads.toString()]
                                                             ^^
  ```

- Warning: `subworkflows/local/pna/generate_reports/main.nf:36:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  data.each { newMeta += it }
                                         ^^
  ```

- Warning: `subworkflows/local/pna/generate_reports/main.nf:89:77`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_experiment_summary = ch_grouped_data.map { it -> it[0] }.combine(Channel.of([]))
                                                                              ^^^^^^^
  ```

- Warning: `subworkflows/local/pna/main.nf:108:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def parquet = data.collect { it[1] }.flatten()
                                           ^^
  ```

- Warning: `subworkflows/local/pna/main.nf:109:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def reports = data.collect { it[2] }.flatten()
                                           ^^
  ```

- Warning: `subworkflows/local/pna/main.nf:114:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          single: it[1].size() == 1
                  ^^
  ```

- Warning: `subworkflows/local/pna/main.nf:115:16`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          multi: it[1].size() > 1
                 ^^
  ```

- Warning: `subworkflows/local/pna/main.nf:177:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_input = Channel.fromPath(params.input)
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pixelator_pipeline/main.nf:33:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pixelator_pipeline/main.nf:123:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              validate_input_samplesheet(inputBaseDir, it)
                                                       ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pixelator_pipeline/main.nf:134:16`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { it.trim() }
                 ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pixelator_pipeline/main.nf:140:16`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { it.trim() }
                 ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pixelator_pipeline/main.nf:327:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      catch (URISyntaxException exc) {
                                ^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_pixelator_pipeline/main.nf:397:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      catch (URISyntaxException exc) {
                                ^^^
  ```

- Warning: `workflows/pixelator.nf:13:5`: Params should be declared at the top-level (i.e. outside the workflow)

  ```nextflow
      params.samplesheet_sha = file(params.input).bytes.digest('sha-1')
      ^^^^^^
  ```

- Warning: `workflows/pixelator.nf:69:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_reads       = ch_samplesheet.map { meta, panel, reads -> [ meta, reads ] }
                                                  ^^^^^
  ```

- Warning: `workflows/pixelator.nf:70:56`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_panel_files = ch_samplesheet.map { meta, panel, reads -> [ meta, panel ] }
                                                         ^^^^^
  ```

- Warning: `workflows/pixelator.nf:109:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { id, meta, panel_files -> [meta, panel_files] }
                 ^^
  ```

- Warning: `workflows/pixelator.nf:157:17`: Variable was declared but not used

  ```nextflow
          ).set { ch_collated_versions }
                  ^^^^^^^^^^^^^^^^^^^^
  ```
