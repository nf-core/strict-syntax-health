# Nextflow lint results

- Generated: 2026-06-16T20:31:21.144084059Z
- Nextflow version: 26.04.3
- Summary: 178 warnings

## :warning: Warnings

- Warning: `modules/local/custom/calculate_gaps/main.nf:20:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/custom/calculate_seqstats/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/custom/create_template/main.nf:20:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/custom/extract_plddt/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/custom/parse_irmsd/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/custom/parse_sim/main.nf:20:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/custom/prepare_multiqc/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/custom/prepare_shiny/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def args         = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/custom/prepare_shiny/main.nf:24:5`: Variable was declared but not used

  ```nextflow
      prefix           = task.ext.prefix ?: "${meta.id}"
      ^^^^^^
  ```

- Warning: `modules/nf-core/clustalo/align/main.nf:60:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/clustalo/guidetree/main.nf:37:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/famsa/guidetree/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/foldmason/createdb/main.nf:37:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/foldmason/easymsa/main.nf:52:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/foldmason/msa2lddtreport/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/kalign/align/main.nf:59:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/mafft/guidetree/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/magus/align/main.nf:47:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/mtmalign/align/main.nf:25:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/muscle5/super5/main.nf:52:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/pigz/compress/main.nf:35:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/pigz/uncompress/main.nf:39:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/tcoffee/alncompare/main.nf:58:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/tcoffee/extractfrompdb/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/tcoffee/irmsd/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/tcoffee/seqreformat/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/tcoffee/tcs/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def args          = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/tcoffee/tcs/main.nf:63:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/upp/align/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def tree_args = tree ? "-t $tree" : ""
          ^^^^^^^^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:40:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_msa      = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:41:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:81:13`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              it[1] != null
              ^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:92:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              clustalo:   it[0]["aligner"] == "CLUSTALO"
                          ^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:93:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              famsa:      it[0]["aligner"] == "FAMSA"
                          ^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:94:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              kalign:     it[0]["aligner"] == "KALIGN"
                          ^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:95:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              learnmsa:   it[0]["aligner"] == "LEARNMSA"
                          ^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:96:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              mafft:      it[0]["aligner"] == "MAFFT"
                          ^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:97:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              magus:      it[0]["aligner"] == "MAGUS"
                          ^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:98:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              muscle5:    it[0]["aligner"] == "MUSCLE5"
                          ^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:99:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              mtmalign:   it[0]["aligner"] == "MTMALIGN"
                          ^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:100:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              regressive: it[0]["aligner"] == "REGRESSIVE"
                          ^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:101:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              tcoffee:    it[0]["aligner"] == "TCOFFEE"
                          ^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:102:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              tcoffee3d:  it[0]["aligner"] == "3DCOFFEE"
                          ^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:103:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              upp:        it[0]["aligner"] == "UPP"
                          ^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:114:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              mtmalign: it[0]["aligner"] == "MTMALIGN"
                        ^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:127:13`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              it.size() == 5
              ^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:134:24`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              foldmason: it[0]["aligner"] == "FOLDMASON"
                         ^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:184:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, fastafile, treefile ->
                               ^^^^^^^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:199:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, fastafile, treefile ->
                               ^^^^^^^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:221:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, fastafile, treefile ->
                               ^^^^^^^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:257:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, fastafile, treefile ->
                               ^^^^^^^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:330:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  merging_id, meta, fastafile, treefile, templatefile, datafiles ->
                  ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:351:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, template, dependency ->
                        ^^^^^^^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:368:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, tree, template, dependency ->
                              ^^^^^^^^
  ```

- Warning: `subworkflows/local/ALIGN/main.nf:387:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter { it[1].size() > 1 }
                        ^^
  ```

- Warning: `subworkflows/local/COMPUTE_TREES/main.nf:16:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_optional_data //channel: [ meta, template, [ /path/to/file1, /path/to/file2, ... ] ]
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/COMPUTE_TREES/main.nf:20:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/COMPUTE_TREES/main.nf:21:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_trees    = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/COMPUTE_TREES/main.nf:33:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              famsa:    it[0]["tree"] == "FAMSA"
                        ^^
  ```

- Warning: `subworkflows/local/COMPUTE_TREES/main.nf:34:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              clustalo: it[0]["tree"] == "CLUSTALO"
                        ^^
  ```

- Warning: `subworkflows/local/COMPUTE_TREES/main.nf:35:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              mafft:    it[0]["tree"] == "MAFFT"
                        ^^
  ```

- Warning: `subworkflows/local/EVALUATE/main.nf:28:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions     = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/EVALUATE/main.nf:29:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      sp_csv          = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/EVALUATE/main.nf:30:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tc_csv          = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/EVALUATE/main.nf:31:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      irmsd_csv       = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/EVALUATE/main.nf:32:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      tcs_csv         = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/EVALUATE/main.nf:33:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      gaps_csv        = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/EVALUATE/main.nf:34:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_eval_summary = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/EVALUATE/main.nf:66:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, csv -> csv
                  ^^^^
  ```

- Warning: `subworkflows/local/EVALUATE/main.nf:87:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, csv ->
                  ^^^^
  ```

- Warning: `subworkflows/local/EVALUATE/main.nf:114:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, csv ->
                  ^^^^
  ```

- Warning: `subworkflows/local/EVALUATE/main.nf:163:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                                      meta, csv -> csv
                                                      ^^^^
  ```

- Warning: `subworkflows/local/EVALUATE/main.nf:169:9`: Variable was declared but not used

  ```nextflow
          versions = ch_versions.mix(CONCAT_IRMSD.out.versions)
          ^^^^^^^^
  ```

- Warning: `subworkflows/local/EVALUATE/main.nf:186:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, csv ->
                  ^^^^
  ```

- Warning: `subworkflows/local/EVALUATE/main.nf:206:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      sp      = sp_csv.map    { meta, csv -> csv }
                                ^^^^
  ```

- Warning: `subworkflows/local/EVALUATE/main.nf:207:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      tc      = tc_csv.map    { meta, csv -> csv }
                                ^^^^
  ```

- Warning: `subworkflows/local/EVALUATE/main.nf:208:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      irmsd   = irmsd_csv.map { meta, csv -> csv }
                                ^^^^
  ```

- Warning: `subworkflows/local/EVALUATE/main.nf:209:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      gaps    = gaps_csv.map  { meta, csv -> csv }
                                ^^^^
  ```

- Warning: `subworkflows/local/EVALUATE/main.nf:210:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      tcs     = tcs_csv.map   { meta, csv -> csv }
                                ^^^^
  ```

- Warning: `subworkflows/local/PREPROCESS/main.nf:10:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/PREPROCESS/main.nf:11:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_preprocessed_data = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/STATS/main.nf:20:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions      = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/STATS/main.nf:21:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      sim_csv          = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/STATS/main.nf:22:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      seqstats_csv     = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/STATS/main.nf:23:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      plddts_csv       = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/STATS/main.nf:24:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_stats_summary = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/STATS/main.nf:39:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, csv ->
                  ^^^^
  ```

- Warning: `subworkflows/local/STATS/main.nf:70:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, csv ->
                  ^^^^
  ```

- Warning: `subworkflows/local/STATS/main.nf:99:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, csv -> csv
                  ^^^^
  ```

- Warning: `subworkflows/local/STATS/main.nf:121:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      sim      = sim_csv.map      { meta, csv -> csv }
                                    ^^^^
  ```

- Warning: `subworkflows/local/STATS/main.nf:122:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      seqstats = seqstats_csv.map { meta, csv -> csv }
                                    ^^^^
  ```

- Warning: `subworkflows/local/STATS/main.nf:123:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      plddts   = plddts_csv.map   { meta, csv -> csv }
                                    ^^^^
  ```

- Warning: `subworkflows/local/STATS/main.nf:139:14`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ].count{ it == true }
               ^^
  ```

- Warning: `subworkflows/local/TEMPLATES/main.nf:12:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/TEMPLATES/main.nf:17:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              template: it[2] != null
                        ^^
  ```

- Warning: `subworkflows/local/TEMPLATES/main.nf:26:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta,optional_data,template ->
                                     ^^^^^^^^
  ```

- Warning: `subworkflows/local/TEMPLATES/main.nf:35:18`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta,optional_data,template ->
                   ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/VISUALIZATION/main.nf:13:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/VISUALIZATION/main.nf:14:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_html     = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/VISUALIZATION/main.nf:25:13`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              it.size() == 4
              ^^
  ```

- Warning: `subworkflows/local/VISUALIZATION/main.nf:28:13`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              tree_meta, meta, msa, tree -> [ meta.subMap(["id"]), meta, msa, tree ]
              ^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      tools             //  string: Path to input tools samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:110:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_input = Channel.fromList([
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:114:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_input = Channel.fromList([
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:118:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_input = Channel.fromList([
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:124:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_input = Channel.fromList(samplesheetToList(params.input, "${projectDir}/assets/schema_input.json"))
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:129:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_tools = Channel.fromList([
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:134:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.fromList(samplesheetToList(params.tools, "${projectDir}/assets/schema_tools.json")).set{ ch_tools }
          ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:404:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          def mutableRow = map.findAll { key, value ->
                                              ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:486:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def traceFile = new File(traceDirPath).listFiles().findAll { it.name.startsWith(filePattern) }.sort { -it.lastModified() }.take(1)[0]
                                                                   ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:486:108`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def traceFile = new File(traceDirPath).listFiles().findAll { it.name.startsWith(filePattern) }.sort { -it.lastModified() }.take(1)[0]
                                                                                                             ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:490:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def traceFileAlign = traceFile.readLines().findAll { it.contains("COMPLETED") && it.contains("MULTIPLESEQUENCEALIGN:ALIGN") }.collect { it.replaceAll("\t", ",") }.join("\n")
                                                           ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:490:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def traceFileAlign = traceFile.readLines().findAll { it.contains("COMPLETED") && it.contains("MULTIPLESEQUENCEALIGN:ALIGN") }.collect { it.replaceAll("\t", ",") }.join("\n")
                                                                                       ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:490:141`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def traceFileAlign = traceFile.readLines().findAll { it.contains("COMPLETED") && it.contains("MULTIPLESEQUENCEALIGN:ALIGN") }.collect { it.replaceAll("\t", ",") }.join("\n")
                                                                                                                                              ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:509:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def map1 = list1.collectEntries { [(it[idKey]): it] }
                                          ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:509:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def map1 = list1.collectEntries { [(it[idKey]): it] }
                                                      ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:551:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          mutableRow.args = mutableRow.tag?.split("args:")?.with { it.size() > 1 ? it[1].trim() : "default" }
                                                                   ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:551:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          mutableRow.args = mutableRow.tag?.split("args:")?.with { it.size() > 1 ? it[1].trim() : "default" }
                                                                                   ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:563:35`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      return cleanedTrace.findAll { it != null }
                                    ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:589:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def trace_co2_csv = mergeListsById(traceCsv.collect { it as Map }, co2Csv, "name")
                                                            ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:627:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def trace_subworkflow = trace.findAll { it.subworkflow == subworkflow }
                                              ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:734:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def data = parseCsv(new File(summary_file).readLines().collect { it.replaceAll("\t", ",") }.join("\n"))
                                                                       ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:777:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              treeMatch = trace_file.traceTrees.find {it.tree == row.tree && it.args_tree_clean == row.args_tree_clean}
                                                      ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:777:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              treeMatch = trace_file.traceTrees.find {it.tree == row.tree && it.args_tree_clean == row.args_tree_clean}
                                                                             ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:779:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              treeMatch = trace_file.traceTrees.find { it.id == row.id && it.tree == row.tree && it.args_tree_clean == row.args_tree_clean}
                                                       ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:779:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              treeMatch = trace_file.traceTrees.find { it.id == row.id && it.tree == row.tree && it.args_tree_clean == row.args_tree_clean}
                                                                          ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:779:96`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              treeMatch = trace_file.traceTrees.find { it.id == row.id && it.tree == row.tree && it.args_tree_clean == row.args_tree_clean}
                                                                                                 ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:782:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def alignMatch = trace_file.traceAlign.find { it.id == row.id && it.tree == row.tree && row.args_tree_clean == it.args_tree_clean && it.aligner == row.aligner && it.args_aligner_clean == row.args_aligner_clean}
                                                        ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:782:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def alignMatch = trace_file.traceAlign.find { it.id == row.id && it.tree == row.tree && row.args_tree_clean == it.args_tree_clean && it.aligner == row.aligner && it.args_aligner_clean == row.args_aligner_clean}
                                                                           ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:782:120`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def alignMatch = trace_file.traceAlign.find { it.id == row.id && it.tree == row.tree && row.args_tree_clean == it.args_tree_clean && it.aligner == row.aligner && it.args_aligner_clean == row.args_aligner_clean}
                                                                                                                         ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:782:142`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def alignMatch = trace_file.traceAlign.find { it.id == row.id && it.tree == row.tree && row.args_tree_clean == it.args_tree_clean && it.aligner == row.aligner && it.args_aligner_clean == row.args_aligner_clean}
                                                                                                                                               ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_multiplesequencealign_pipeline/main.nf:782:171`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def alignMatch = trace_file.traceAlign.find { it.id == row.id && it.tree == row.tree && row.args_tree_clean == it.args_tree_clean && it.aligner == row.aligner && it.args_aligner_clean == row.args_aligner_clean}
                                                                                                                                                                            ^^
  ```

- Warning: `subworkflows/nf-core/utils_nextflow_pipeline/main.nf:43:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:20:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      valid_config = valid_config
      ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:72:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:61:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      multiqc_config   // string: path to MultiQC config file or list of paths if multiple config files
      ^^^^^^^^^^^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:62:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      multiqc_logo     // string: path to MultiQC logo file
      ^^^^^^^^^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:63:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      multiqc_methods_description // string: path to MultiQC methods description file
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:69:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_report            = Channel.empty()
                                     ^^^^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:70:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      evaluation_summary           = Channel.empty()
                                     ^^^^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:71:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      stats_summary                = Channel.empty()
                                     ^^^^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:72:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      stats_and_evaluation_summary = Channel.empty()
                                     ^^^^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:73:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_refs                      = Channel.empty()
                                     ^^^^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:74:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_templates                 = Channel.empty()
                                     ^^^^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:75:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_optional_data             = Channel.empty()
                                     ^^^^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:78:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it[1].size() > 0}
                    ^^
  ```

- Warning: `workflows/multiplesequencealign.nf:80:26`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, fasta, ref, str, template ->
                           ^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:80:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, fasta, ref, str, template ->
                                ^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:80:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, fasta, ref, str, template ->
                                     ^^^^^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:86:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it[2].size() > 0}
                    ^^
  ```

- Warning: `workflows/multiplesequencealign.nf:88:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, fasta, ref, str, template ->
                    ^^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:88:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, fasta, ref, str, template ->
                                ^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:88:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, fasta, ref, str, template ->
                                     ^^^^^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:94:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it[4].size() > 0}
                    ^^
  ```

- Warning: `workflows/multiplesequencealign.nf:96:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, fasta, ref, str, template ->
                    ^^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:96:26`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, fasta, ref, str, template ->
                           ^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:96:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, fasta, ref, str, template ->
                                ^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:123:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              pdbs_dir = Channel.fromPath(params.pdbs_dir)
                         ^^^^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:128:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .map { meta, dir -> [ file(dir).listFiles() ] }
                         ^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:136:42`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              optional_data_to_be_mapped = Channel.fromPath(params.pdbs_dir+"/**")
                                           ^^^^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:162:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .map { dep_id, dep, fasta_id -> [ fasta_id, dep ] }
                         ^^^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:172:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, fasta, ref, str, template ->
                        ^^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:172:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, fasta, ref, str, template ->
                               ^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:172:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, fasta, ref, str, template ->
                                         ^^^^^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:175:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter { it[1].size() > 0 }
                        ^^
  ```

- Warning: `workflows/multiplesequencealign.nf:182:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  compressed:   it[1].endsWith('.tar.gz')
                                ^^
  ```

- Warning: `workflows/multiplesequencealign.nf:205:13`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              it[-1] == null
              ^^
  ```

- Warning: `workflows/multiplesequencealign.nf:245:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it[3]["aligner"] == "3DCOFFEE" }
                    ^^
  ```

- Warning: `workflows/multiplesequencealign.nf:252:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_optional_data_template = Channel.empty()
                                  ^^^^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:266:13`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              it[-1] == null
              ^^
  ```

- Warning: `workflows/multiplesequencealign.nf:313:80`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ALIGN.out.msa.collectFile(keepHeader: true, skip: 1,sort: true){ meta, msa ->
                                                                                 ^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:314:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def content =  meta.keySet().collect{it}.join(",")
                                                   ^^
  ```

- Warning: `workflows/multiplesequencealign.nf:316:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              content += meta.values().collect{it}.join(",")
                                               ^^
  ```

- Warning: `workflows/multiplesequencealign.nf:331:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          stats_summary_csv = stats_summary.map{ meta, csv -> csv }
                                                 ^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:332:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          eval_summary_csv  = evaluation_summary.map{ meta, csv -> csv }
                                                      ^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:349:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          shiny_app = Channel.fromPath(params.shiny_app)
                      ^^^^^^^
  ```

- Warning: `workflows/multiplesequencealign.nf:408:92`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(PREPARE_MULTIQC.out.multiqc_table.collect{ it[1] }.ifEmpty([]))
                                                                                             ^^
  ```
