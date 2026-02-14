# Nextflow lint results

- Generated: 2026-02-14T00:20:09.330661064Z
- Nextflow version: 26.01.1-edge
- Summary: 13 errors, 48 warnings

## :x: Errors

- Error: `main.nf:18:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/differentialabundance/workflows/differentialabundance.nf'

  ```nextflow
  include { DIFFERENTIALABUNDANCE   } from './workflows/differentialabundance'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:19:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/differentialabundance/subworkflows/local/utils_nfcore_differentialabundance_pipeline/main.nf'

  ```nextflow
  include { PIPELINE_INITIALISATION } from './subworkflows/local/utils_nfcore_differentialabundance_pipeline'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:20:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/differentialabundance/subworkflows/local/utils_nfcore_differentialabundance_pipeline/main.nf'

  ```nextflow
  include { PIPELINE_COMPLETION     } from './subworkflows/local/utils_nfcore_differentialabundance_pipeline'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:21:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/differentialabundance/subworkflows/local/utils_nfcore_differentialabundance_pipeline/main.nf'

  ```nextflow
  include { getGenomeAttribute      } from './subworkflows/local/utils_nfcore_differentialabundance_pipeline'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:29:14`: `getGenomeAttribute` is not defined

  ```nextflow
  params.gtf = getGenomeAttribute('gtf')
               ^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:50:5`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      DIFFERENTIALABUNDANCE (
      ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:67:5`: `PIPELINE_INITIALISATION` is not defined

  ```nextflow
      PIPELINE_INITIALISATION (
      ^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:84:9`: `PIPELINE_INITIALISATION` is not defined

  ```nextflow
          PIPELINE_INITIALISATION.out.paramsets
          ^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:90:5`: `PIPELINE_COMPLETION` is not defined

  ```nextflow
      PIPELINE_COMPLETION (
      ^^^^^^^^^^^^^^^^^^^
  ```

- Error: `modules/nf-core/quartonotebook/main.nf:45:5`: `yamlBuilder` is not defined

  ```nextflow
      yamlBuilder(notebook_parameters)
      ^^^^^^^^^^^
  ```

- Error: `modules/nf-core/shinyngs/app/tests/nextflow.config:6:32`: Unexpected input: ':'

  ```nextflow
      withName: test_shinyngs_app:SHINYNGS_APP {
                                 ^
  ```

- Error: `subworkflows/local/utils_nfcore_differentialabundance_pipeline/main.nf:434:43`: Unexpected input: '('

  ```nextflow
      yaml_content = yaml_content.replaceAll(/\$projectDir/, projectDir.toString())
                                            ^
  ```

- Error: `workflows/differentialabundance.nf:214:96`: Unexpected input: '='

  ```nextflow
      ch_proteus_raw = prepareModuleOutput(PROTEUS.out.raw_tab, ch_paramsets, meta_keys_to_remove=['contrast'])
                                                                                                 ^
  ```

## :warning: Warnings

- Warning: `modules/nf-core/custom/filterdifferentialtable/main.nf:25:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/gunzip/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/shinyngs/app/main.nf:56:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/shinyngs/staticexploratory/main.nf:51:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/nf-core/abundance_differential_filter/main.nf:34:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/abundance_differential_filter/main.nf:93:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          norm_inputs.contrasts_for_norm_with_formula.filter{it[0].differential_method == 'limma'},
                                                             ^^
  ```

- Warning: `subworkflows/nf-core/abundance_differential_filter/main.nf:94:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          norm_inputs.samples_and_matrix.filter{it[0].differential_method == 'limma'}
                                                ^^
  ```

- Warning: `subworkflows/nf-core/abundance_differential_filter/main.nf:100:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          inputs.contrasts_for_diff_with_formula.filter{ it[0].differential_method == 'limma' },
                                                         ^^
  ```

- Warning: `subworkflows/nf-core/abundance_differential_filter/main.nf:101:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          inputs.samples_and_matrix.filter{ it[0].differential_method == 'limma' }
                                            ^^
  ```

- Warning: `subworkflows/nf-core/abundance_differential_filter/main.nf:118:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          norm_inputs.contrasts_for_norm_with_formula.filter{it[0].differential_method == 'deseq2'},
                                                             ^^
  ```

- Warning: `subworkflows/nf-core/abundance_differential_filter/main.nf:119:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          norm_inputs.samples_and_matrix.filter{it[0].differential_method == 'deseq2'},
                                                ^^
  ```

- Warning: `subworkflows/nf-core/abundance_differential_filter/main.nf:120:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          norm_inputs.control_features.filter{it[0].differential_method == 'deseq2'},
                                              ^^
  ```

- Warning: `subworkflows/nf-core/abundance_differential_filter/main.nf:121:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          norm_inputs.transcript_length.filter{it[0].differential_method == 'deseq2'}
                                               ^^
  ```

- Warning: `subworkflows/nf-core/abundance_differential_filter/main.nf:127:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          inputs.contrasts_for_diff_with_formula.filter{it[0].differential_method == 'deseq2'},
                                                        ^^
  ```

- Warning: `subworkflows/nf-core/abundance_differential_filter/main.nf:128:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          inputs.samples_and_matrix.filter{it[0].differential_method == 'deseq2'},
                                           ^^
  ```

- Warning: `subworkflows/nf-core/abundance_differential_filter/main.nf:129:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          inputs.control_features.filter{it[0].differential_method == 'deseq2'},
                                         ^^
  ```

- Warning: `subworkflows/nf-core/abundance_differential_filter/main.nf:130:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          inputs.transcript_length.filter{it[0].differential_method == 'deseq2'}
                                          ^^
  ```

- Warning: `subworkflows/nf-core/abundance_differential_filter/main.nf:143:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          inputs.contrasts_for_diff.filter{it[0].differential_method == 'propd'},
                                           ^^
  ```

- Warning: `subworkflows/nf-core/abundance_differential_filter/main.nf:144:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          inputs.samples_and_matrix.filter { it[0].differential_method == 'propd' }
                                             ^^
  ```

- Warning: `subworkflows/nf-core/abundance_differential_filter/main.nf:166:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          norm_inputs.contrasts_for_norm_with_formula.filter{it[0].differential_method == 'dream'},
                                                             ^^
  ```

- Warning: `subworkflows/nf-core/abundance_differential_filter/main.nf:167:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          norm_inputs.samples_and_matrix.filter{it[0].differential_method == 'dream'}
                                                ^^
  ```

- Warning: `subworkflows/nf-core/abundance_differential_filter/main.nf:172:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          inputs.samples_and_matrix.filter{ it[0].differential_method == 'dream' }
                                            ^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:36:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:58:62`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def criteria = multiMapCriteria { meta, input, genesets, background, method, samplesheet, featuresheet, features_id, features_symbol, meta_contrast, variable, reference, target, formula, comparison ->
                                                               ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:58:154`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def criteria = multiMapCriteria { meta, input, genesets, background, method, samplesheet, featuresheet, features_id, features_symbol, meta_contrast, variable, reference, target, formula, comparison ->
                                                                                                                                                           ^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:58:164`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def criteria = multiMapCriteria { meta, input, genesets, background, method, samplesheet, featuresheet, features_id, features_symbol, meta_contrast, variable, reference, target, formula, comparison ->
                                                                                                                                                                     ^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:58:175`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def criteria = multiMapCriteria { meta, input, genesets, background, method, samplesheet, featuresheet, features_id, features_symbol, meta_contrast, variable, reference, target, formula, comparison ->
                                                                                                                                                                                ^^^^^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:58:183`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def criteria = multiMapCriteria { meta, input, genesets, background, method, samplesheet, featuresheet, features_id, features_symbol, meta_contrast, variable, reference, target, formula, comparison ->
                                                                                                                                                                                        ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:58:192`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def criteria = multiMapCriteria { meta, input, genesets, background, method, samplesheet, featuresheet, features_id, features_symbol, meta_contrast, variable, reference, target, formula, comparison ->
                                                                                                                                                                                                 ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:75:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, contrastMap, variable, reference, target, formula, comparison ->
                    ^^^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:75:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, contrastMap, variable, reference, target, formula, comparison ->
                          ^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:75:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, contrastMap, variable, reference, target, formula, comparison ->
                                                 ^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:75:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, contrastMap, variable, reference, target, formula, comparison ->
                                                            ^^^^^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:75:67`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, contrastMap, variable, reference, target, formula, comparison ->
                                                                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:75:76`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, contrastMap, variable, reference, target, formula, comparison ->
                                                                             ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:80:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter{ it[4] == 'gsea' }
                   ^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:91:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_input_for_other.input.filter{ it[0].functional_method == 'gprofiler2' },
                                           ^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:92:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_input_for_other.genesets.filter{ it[0].functional_method == 'gprofiler2'},
                                              ^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:93:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_input_for_other.background.filter{ it[0].functional_method == 'gprofiler2'}
                                                ^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:119:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_input_for_gsea.map{ tuple(it[0].reference, it[0].target) },
                                       ^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:119:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_input_for_gsea.map{ tuple(it[0].reference, it[0].target) },
                                                        ^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:127:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_input_for_other.input.filter{ it[0].functional_method == 'decoupler' },
                                           ^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:128:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_input_for_other.genesets.filter{ it[0].functional_method == 'decoupler'},
                                              ^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:129:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_input_for_other.features.filter{ it[0].functional_method == 'decoupler'}
                                              ^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:130:41`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map{ meta, features_sheet, features_id, features_symbol -> [meta, features_sheet] }
                                          ^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:130:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map{ meta, features_sheet, features_id, features_symbol -> [meta, features_sheet] }
                                                       ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:138:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_input_for_other.input.filter{ it[0].functional_method == 'grea' },
                                           ^^
  ```

- Warning: `subworkflows/nf-core/differential_functional_enrichment/main.nf:139:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_input_for_other.genesets.filter{ it[0].functional_method == 'grea' }
                                              ^^
  ```
