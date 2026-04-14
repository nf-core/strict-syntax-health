# Nextflow lint results

- Generated: 2026-04-14T00:31:43.474118016Z
- Nextflow version: 26.03.2-edge
- Summary: 75 errors, 9 warnings

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

- Error: `main.nf:57:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      affy_cel_files             = DIFFERENTIALABUNDANCE.out.affy_cel_files
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:58:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      affy_raw_expression        = DIFFERENTIALABUNDANCE.out.affy_raw_expression
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:59:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      affy_norm_expression       = DIFFERENTIALABUNDANCE.out.affy_norm_expression
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:60:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      affy_annotation            = DIFFERENTIALABUNDANCE.out.affy_annotation
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:61:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      affy_raw_rds               = DIFFERENTIALABUNDANCE.out.affy_raw_rds
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:64:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      proteus_raw                = DIFFERENTIALABUNDANCE.out.proteus_raw
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:65:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      proteus_norm               = DIFFERENTIALABUNDANCE.out.proteus_norm
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:66:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      proteus_plots              = DIFFERENTIALABUNDANCE.out.proteus_plots
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:67:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      proteus_raw_rdata          = DIFFERENTIALABUNDANCE.out.proteus_raw_rdata
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:68:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      proteus_norm_rdata         = DIFFERENTIALABUNDANCE.out.proteus_norm_rdata
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:69:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      proteus_session_info       = DIFFERENTIALABUNDANCE.out.proteus_session_info
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:72:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      geo_expression             = DIFFERENTIALABUNDANCE.out.geo_expression
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:73:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      geo_annotation             = DIFFERENTIALABUNDANCE.out.geo_annotation
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:74:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      geo_rds                    = DIFFERENTIALABUNDANCE.out.geo_rds
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:77:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gtf_annotation             = DIFFERENTIALABUNDANCE.out.gtf_annotation
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:80:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      diff_results               = DIFFERENTIALABUNDANCE.out.diff_results
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:81:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      diff_results_filtered      = DIFFERENTIALABUNDANCE.out.diff_results_filtered
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:82:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      diff_normalised_matrix     = DIFFERENTIALABUNDANCE.out.diff_normalised_matrix
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:83:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      diff_variance_stabilised   = DIFFERENTIALABUNDANCE.out.diff_variance_stabilised
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:84:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      diff_size_factors          = DIFFERENTIALABUNDANCE.out.diff_size_factors
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:85:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      diff_dispersion_plot       = DIFFERENTIALABUNDANCE.out.diff_dispersion_plot
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:86:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      diff_md_plot               = DIFFERENTIALABUNDANCE.out.diff_md_plot
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:87:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      diff_rdata                 = DIFFERENTIALABUNDANCE.out.diff_rdata
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:88:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      diff_session_info          = DIFFERENTIALABUNDANCE.out.diff_session_info
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:89:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      diff_annotated             = DIFFERENTIALABUNDANCE.out.diff_annotated
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:92:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gsea_report_tsv            = DIFFERENTIALABUNDANCE.out.gsea_report_tsv
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:93:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gsea_report_html           = DIFFERENTIALABUNDANCE.out.gsea_report_html
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:94:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gsea_index_html            = DIFFERENTIALABUNDANCE.out.gsea_index_html
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:95:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gsea_heat_map_corr_plot    = DIFFERENTIALABUNDANCE.out.gsea_heat_map_corr_plot
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:96:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gsea_ranked_gene_list      = DIFFERENTIALABUNDANCE.out.gsea_ranked_gene_list
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:97:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gsea_gene_set_sizes        = DIFFERENTIALABUNDANCE.out.gsea_gene_set_sizes
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:98:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gsea_histogram             = DIFFERENTIALABUNDANCE.out.gsea_histogram
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:99:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gsea_heatmap               = DIFFERENTIALABUNDANCE.out.gsea_heatmap
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:100:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gsea_pvalues_vs_nes_plot   = DIFFERENTIALABUNDANCE.out.gsea_pvalues_vs_nes_plot
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:101:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gsea_ranked_list_corr      = DIFFERENTIALABUNDANCE.out.gsea_ranked_list_corr
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:102:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gsea_butterfly_plot        = DIFFERENTIALABUNDANCE.out.gsea_butterfly_plot
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:103:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gsea_gene_set_tsv          = DIFFERENTIALABUNDANCE.out.gsea_gene_set_tsv
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:104:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gsea_gene_set_html         = DIFFERENTIALABUNDANCE.out.gsea_gene_set_html
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:105:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gsea_gene_set_heatmap      = DIFFERENTIALABUNDANCE.out.gsea_gene_set_heatmap
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:106:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gsea_gene_set_enplot       = DIFFERENTIALABUNDANCE.out.gsea_gene_set_enplot
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:107:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gsea_gene_set_dist         = DIFFERENTIALABUNDANCE.out.gsea_gene_set_dist
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:108:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gsea_snapshot              = DIFFERENTIALABUNDANCE.out.gsea_snapshot
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:109:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gsea_archive               = DIFFERENTIALABUNDANCE.out.gsea_archive
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:110:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gsea_rpt                   = DIFFERENTIALABUNDANCE.out.gsea_rpt
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:113:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gprofiler2_html            = DIFFERENTIALABUNDANCE.out.gprofiler2_html
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:114:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gprofiler2_all_enrichment  = DIFFERENTIALABUNDANCE.out.gprofiler2_all_enrichment
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:115:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gprofiler2_sub_enrichment  = DIFFERENTIALABUNDANCE.out.gprofiler2_sub_enrichment
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:116:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gprofiler2_plot_png        = DIFFERENTIALABUNDANCE.out.gprofiler2_plot_png
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:117:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gprofiler2_sub_plot        = DIFFERENTIALABUNDANCE.out.gprofiler2_sub_plot
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:118:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gprofiler2_rds             = DIFFERENTIALABUNDANCE.out.gprofiler2_rds
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:119:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      gprofiler2_filtered_gmt    = DIFFERENTIALABUNDANCE.out.gprofiler2_filtered_gmt
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:122:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      decoupler_estimate         = DIFFERENTIALABUNDANCE.out.decoupler_estimate
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:123:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      decoupler_pvals            = DIFFERENTIALABUNDANCE.out.decoupler_pvals
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:124:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      decoupler_png              = DIFFERENTIALABUNDANCE.out.decoupler_png
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:127:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      functional_session_info    = DIFFERENTIALABUNDANCE.out.functional_session_info
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:130:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      plot_exploratory           = DIFFERENTIALABUNDANCE.out.plot_exploratory
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:131:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      plot_volcanos              = DIFFERENTIALABUNDANCE.out.plot_volcanos
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:134:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      shinyngs_data              = DIFFERENTIALABUNDANCE.out.shinyngs_data
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:135:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      shinyngs_app_file          = DIFFERENTIALABUNDANCE.out.shinyngs_app_file
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:138:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      report_html                = DIFFERENTIALABUNDANCE.out.report_html
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:139:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      report_bundle              = DIFFERENTIALABUNDANCE.out.report_bundle
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:142:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      nfcore_versions            = DIFFERENTIALABUNDANCE.out.nfcore_versions
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:143:34`: `DIFFERENTIALABUNDANCE` is not defined

  ```nextflow
      collated_versions          = DIFFERENTIALABUNDANCE.out.collated_versions
                                   ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:159:5`: `PIPELINE_INITIALISATION` is not defined

  ```nextflow
      PIPELINE_INITIALISATION (
      ^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:176:9`: `PIPELINE_INITIALISATION` is not defined

  ```nextflow
          PIPELINE_INITIALISATION.out.paramsets
          ^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:182:5`: `PIPELINE_COMPLETION` is not defined

  ```nextflow
      PIPELINE_COMPLETION (
      ^^^^^^^^^^^^^^^^^^^
  ```

- Error: `modules/nf-core/quartonotebook/main.nf:45:5`: `yamlBuilder` is not defined

  ```nextflow
      yamlBuilder(notebook_parameters)
      ^^^^^^^^^^^
  ```

- Error: `subworkflows/local/utils_nfcore_differentialabundance_pipeline/main.nf:441:43`: Unexpected input: '('

  ```nextflow
      yaml_content = yaml_content.replaceAll(/\$projectDir/, projectDir.toString())
                                            ^
  ```

- Error: `workflows/differentialabundance.nf:213:96`: Unexpected input: '='

  ```nextflow
      ch_proteus_raw = prepareModuleOutput(PROTEUS.out.raw_tab, ch_paramsets, meta_keys_to_remove=['contrast'])
                                                                                                 ^
  ```

## :warning: Warnings

- Warning: `main.nf:278:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          path { name, meta, file ->
                             ^^^^
  ```

- Warning: `main.nf:328:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          path { name, meta, file ->
                             ^^^^
  ```

- Warning: `main.nf:388:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          path { name, meta, file ->
                 ^^^^
  ```

- Warning: `main.nf:393:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          path { name, meta, file ->
                 ^^^^
  ```

- Warning: `main.nf:398:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          path { name, meta, file ->
                 ^^^^
  ```

- Warning: `main.nf:398:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          path { name, meta, file ->
                       ^^^^
  ```

- Warning: `modules/nf-core/gunzip/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/shinyngs/staticexploratory/main.nf:51:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```
