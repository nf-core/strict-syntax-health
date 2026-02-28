# Nextflow lint results

- Generated: 2026-02-28T00:19:51.810055465Z
- Nextflow version: 26.01.1-edge
- Summary: 18 errors, 49 warnings

## :x: Errors

- Error: `conf/base.config:61:29`: Unexpected input: ':'

  ```nextflow
      withName:NFCORE_MHCQUANT:MHCQUANT:PREPARE_SPECTRA:TDF2MZML {
                              ^
  ```

- Error: `conf/modules.config:277:17`: Unexpected input: ':'

  ```nextflow
          withName: 'NFCORE_MHCQUANT:MHCQUANT:QUANT:OPENMS_IDSCORESWITCHER' {
                  ^
  ```

- Error: `main.nf:19:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/mhcquant/subworkflows/local/utils_nfcore_mhcquant_pipeline/main.nf'

  ```nextflow
  include { PIPELINE_INITIALISATION } from './subworkflows/local/utils_nfcore_mhcquant_pipeline'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:20:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/mhcquant/subworkflows/local/utils_nfcore_mhcquant_pipeline/main.nf'

  ```nextflow
  include { PIPELINE_COMPLETION     } from './subworkflows/local/utils_nfcore_mhcquant_pipeline'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:60:5`: `PIPELINE_INITIALISATION` is not defined

  ```nextflow
      PIPELINE_INITIALISATION (
      ^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:76:9`: `PIPELINE_INITIALISATION` is not defined

  ```nextflow
          PIPELINE_INITIALISATION.out.samplesheet,
          ^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:77:9`: `PIPELINE_INITIALISATION` is not defined

  ```nextflow
          PIPELINE_INITIALISATION.out.fasta
          ^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:82:5`: `PIPELINE_COMPLETION` is not defined

  ```nextflow
      PIPELINE_COMPLETION (
      ^^^^^^^^^^^^^^^^^^^
  ```

- Error: `modules/local/ms2rescore/main.nf:11:5`: Invalid process directive

  ```nextflow
      containerOptions = (workflow.containerEngine == 'docker') ? '-u $(id -u) -e "HOME=${HOME}" -v /etc/passwd:/etc/passwd:ro -v /etc/shadow:/etc/shadow:ro -v /etc/group:/etc/group:ro -v $HOME:$HOME' : ''
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `nextflow.config:234:25`: Invalid include source: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/mhcquant/conf/test_percolator.config'

  ```nextflow
      test_percolator   { includeConfig 'conf/test_percolator.config'   }
                          ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `nextflow.config:236:25`: Invalid include source: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/mhcquant/conf/test_epicore.config'

  ```nextflow
      test_epicore      { includeConfig 'conf/test_epicore.config'      }
                          ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/quant/main.nf:18:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  def sortById = { a, b -> a.id <=> b.id }
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/quant/main.nf:77:30`: `mzml` is already declared

  ```nextflow
                  .map { meta, mzml, idxml -> [ groupKey([id: "${meta.sample}_${meta.condition}"], meta.group_count), meta, mzml, idxml] }
                               ^^^^
  ```

- Error: `subworkflows/local/quant/main.nf:79:42`: `mzml` is already declared

  ```nextflow
                  .map { group_meta, meta, mzml, idxml -> [group_meta, meta, mzml, idxml] }
                                           ^^^^
  ```

- Error: `subworkflows/local/quant/main.nf:81:42`: `mzml` is already declared

  ```nextflow
                  .map { group_meta, meta, mzml, idxml, merged_idxml -> [meta, mzml, idxml, merged_idxml] }
                                           ^^^^
  ```

- Error: `subworkflows/local/utils_nfcore_mhcquant_pipeline/main.nf:255:52`: Unexpected input: '/'

  ```nextflow
          def cliOverride = (workflow.commandLine =~ /--${key}[\s=]/).find()
                                                     ^
  ```

- Error: `workflows/mhcquant.nf:45:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/mhcquant/subworkflows/local/utils_nfcore_mhcquant_pipeline/main.nf'

  ```nextflow
  include { methodsDescriptionText                         } from '../subworkflows/local/utils_nfcore_mhcquant_pipeline'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/mhcquant.nf:278:9`: `methodsDescriptionText` is not defined

  ```nextflow
          methodsDescriptionText(ch_multiqc_custom_methods_description))
          ^^^^^^^^^^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `modules/local/epicore/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/openms/idmassaccuracy/main.nf:35:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/openms/mapaligneridentification/main.nf:22:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def out_names = idxmls.collect { it.baseName.replace('_fdr_filtered','')+'.trafoXML' }.join(' ')
                                       ^^
  ```

- Warning: `modules/local/openms/maprttransformer/main.nf:23:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def fileExt = alignment_file.collect { it.name.tokenize("\\.")[1] }.join(' ')
                                             ^^
  ```

- Warning: `modules/local/openms/maprttransformer/main.nf:36:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def fileExt = alignment_file.collect { it.name.tokenize("\\.")[1] }.join(' ')
                                             ^^
  ```

- Warning: `modules/local/openms/psmfeatureextractor/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def extra_features = ""
          ^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/pyopenms/chromatogramextractor/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args  ?: ''
          ^^^^
  ```

- Warning: `modules/local/pyopenms/ionannotator/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/openms/decoydatabase/main.nf:33:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/openms/filefilter/main.nf:37:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/openms/idfilter/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/openms/idfilter/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def filter = filter_file ? "${filter_citerion} ${filter_file}" : ""
          ^^^^^^
  ```

- Warning: `modules/nf-core/openms/idmerger/main.nf:33:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/openms/idripper/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/openms/idripper/main.nf:33:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/openms/idscoreswitcher/main.nf:34:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/openms/peakpickerhires/main.nf:33:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/openms/peptideindexer/main.nf:36:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/openmsthirdparty/cometadapter/main.nf:36:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/map_alignment/main.nf:22:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .flatMap { group_meta, metas -> metas }
                         ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/map_alignment/main.nf:25:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      .flatMap { group_meta, trafoxmls -> [trafoxmls].flatten().collect { trafoxml -> [[spectra: trafoxml.baseName], trafoxml] } })
                                 ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/map_alignment/main.nf:26:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { spectra, meta, trafoxml -> [meta, trafoxml] }
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/map_alignment/main.nf:35:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .flatMap { group_meta, idxmls -> [idxmls].flatten().collect { idxml -> [[spectra: idxml.baseName.replace("_fdr_filtered","")], idxml] } }
                         ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/map_alignment/main.nf:37:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      .flatMap { group_meta, metas -> metas }
                                 ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/map_alignment/main.nf:39:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { group_meta, idxml, meta -> [meta, idxml] }
                     ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/process_feature/main.nf:23:29`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      single: it[1].size() == 1
                              ^^
  ```

- Warning: `subworkflows/local/process_feature/main.nf:24:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      multiple: it[1].size() > 1
                                ^^
  ```

- Warning: `subworkflows/local/quant/main.nf:18:5`: Variable was declared but not used

  ```nextflow
  def sortById = { a, b -> a.id <=> b.id }
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/quant/main.nf:33:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .flatMap { group_meta, idxmls -> [idxmls].flatten().collect { idxml -> [[spectra: idxml.baseName], idxml] } }
                         ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/quant/main.nf:36:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      .flatMap { group_meta, metas -> metas }
                                 ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/quant/main.nf:38:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { spectra, idxmls, meta -> [meta, idxmls] }
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/quant/main.nf:53:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { group_meta, meta, idxml, q_value -> [meta, idxml, q_value] }
                     ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/quant/main.nf:81:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .map { group_meta, meta, mzml, idxml, merged_idxml -> [meta, mzml, idxml, merged_idxml] }
                         ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/rescore/main.nf:53:99`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(OPENMS_PERCOLATORADAPTER.out.feature_weights.map{ meta, feature_weights -> feature_weights })
                                                                                                    ^^^^
  ```

- Warning: `subworkflows/local/rescore/main.nf:80:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      .map { preset, group_meta, local_idxml, global_filtered_idxml ->
                             ^^^^^^
  ```

- Warning: `subworkflows/local/speclib/main.nf:45:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, psmpkl -> [[id: "global"], psmpkl] }
                     ^^^^
  ```

- Warning: `subworkflows/local/speclib/main.nf:49:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, peakpkl -> [[id: "global"], peakpkl] }
                     ^^^^
  ```

- Warning: `workflows/mhcquant.nf:84:89`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(PYOPENMS_CHROMATOGRAMEXTRACTOR.out.csv.map{ meta, mzml -> mzml })
                                                                                          ^^^^
  ```

- Warning: `workflows/mhcquant.nf:88:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_clean_mzml_file.combine(ch_decoy_db.map{ meta, fasta -> [fasta] }) :
                                                      ^^^^
  ```

- Warning: `workflows/mhcquant.nf:92:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { groupKey, meta, mzml, fasta -> [meta, mzml, fasta] }
                     ^^^^^^^^
  ```

- Warning: `workflows/mhcquant.nf:99:74`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          OPENMSTHIRDPARTY_COMETADAPTER.out.idxml.combine(ch_decoy_db.map{ meta, fasta -> [fasta] }) :
                                                                           ^^^^
  ```

- Warning: `workflows/mhcquant.nf:103:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { groupKey, meta, idxml, fasta -> [meta, idxml, fasta] }
                     ^^^^^^^^
  ```

- Warning: `workflows/mhcquant.nf:109:85`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(OPENMS_IDMASSACCURACY.out.frag_err.map{ meta, frag_err -> frag_err })
                                                                                      ^^^^
  ```

- Warning: `workflows/mhcquant.nf:113:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, idxml -> [ groupKey([id: "${meta.sample}_${meta.condition}"], meta.group_count), meta] }
                       ^^^^^
  ```

- Warning: `workflows/mhcquant.nf:130:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { gkey, metas, mzmls, idxml ->
                     ^^^^
  ```

- Warning: `workflows/mhcquant.nf:149:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .map { groupKey, meta, comet_idxml, fdr_filtered_idxml -> [meta, comet_idxml, fdr_filtered_idxml] }
                         ^^^^^^^^
  ```

- Warning: `workflows/mhcquant.nf:155:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, idxml -> idxml.countLines() > 130 }
                        ^^^^
  ```

- Warning: `workflows/mhcquant.nf:225:88`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          params.epicore ? EPICORE.out.stats : SUMMARIZE_RESULTS.out.epicore_input.map { meta, tsv, stats -> stats }
                                                                                         ^^^^
  ```

- Warning: `workflows/mhcquant.nf:225:94`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          params.epicore ? EPICORE.out.stats : SUMMARIZE_RESULTS.out.epicore_input.map { meta, tsv, stats -> stats }
                                                                                               ^^^
  ```
