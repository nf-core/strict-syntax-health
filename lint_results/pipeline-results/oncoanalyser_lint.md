# Nextflow lint results

- Generated: 2026-08-04T00:32:41.669469543Z
- Nextflow version: 26.07.0-edge
- Summary: 30 errors, 104 warnings

## :x: Errors

- Error: `subworkflows/local/read_alignment_dna/main.nf:186:17`: Unexpected input: '\*'

  ```nextflow
                  *:meta_aln,
                  ^
  ```

- Error: `subworkflows/local/read_alignment_rna/main.nf:58:17`: Unexpected input: '\*'

  ```nextflow
                  *:meta_fastq,
                  ^
  ```

- Error: `workflows/panel_resource_creation.nf:15:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/oncoanalyser/subworkflows/local/read_alignment_dna/main.nf'

  ```nextflow
  include { READ_ALIGNMENT_DNA                      } from '../subworkflows/local/read_alignment_dna'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/panel_resource_creation.nf:16:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/oncoanalyser/subworkflows/local/read_alignment_rna/main.nf'

  ```nextflow
  include { READ_ALIGNMENT_RNA                      } from '../subworkflows/local/read_alignment_rna'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/panel_resource_creation.nf:117:5`: `READ_ALIGNMENT_DNA` is not defined

  ```nextflow
      READ_ALIGNMENT_DNA(
      ^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/panel_resource_creation.nf:125:5`: `READ_ALIGNMENT_RNA` is not defined

  ```nextflow
      READ_ALIGNMENT_RNA(
      ^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/panel_resource_creation.nf:132:30`: `READ_ALIGNMENT_DNA` is not defined

  ```nextflow
      ch_align_dna_tumor_out = READ_ALIGNMENT_DNA.out.tumor
                               ^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/panel_resource_creation.nf:133:31`: `READ_ALIGNMENT_DNA` is not defined

  ```nextflow
      ch_align_dna_normal_out = READ_ALIGNMENT_DNA.out.normal
                                ^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/panel_resource_creation.nf:134:30`: `READ_ALIGNMENT_RNA` is not defined

  ```nextflow
      ch_align_rna_tumor_out = READ_ALIGNMENT_RNA.out.tumor
                               ^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/purity_estimate.nf:11:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/oncoanalyser/subworkflows/local/read_alignment_dna/main.nf'

  ```nextflow
  include { READ_ALIGNMENT_DNA              } from '../subworkflows/local/read_alignment_dna'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/purity_estimate.nf:96:9`: `READ_ALIGNMENT_DNA` is not defined

  ```nextflow
          READ_ALIGNMENT_DNA(
          ^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/purity_estimate.nf:104:61`: `READ_ALIGNMENT_DNA` is not defined

  ```nextflow
          ch_align_dna_tumor_out = ch_align_dna_tumor_out.mix(READ_ALIGNMENT_DNA.out.tumor)
                                                              ^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/purity_estimate.nf:105:63`: `READ_ALIGNMENT_DNA` is not defined

  ```nextflow
          ch_align_dna_normal_out = ch_align_dna_normal_out.mix(READ_ALIGNMENT_DNA.out.normal)
                                                                ^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/purity_estimate.nf:106:61`: `READ_ALIGNMENT_DNA` is not defined

  ```nextflow
          ch_align_dna_donor_out = ch_align_dna_donor_out.mix(READ_ALIGNMENT_DNA.out.donor)
                                                              ^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/targeted.nf:24:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/oncoanalyser/subworkflows/local/read_alignment_dna/main.nf'

  ```nextflow
  include { READ_ALIGNMENT_DNA       } from '../subworkflows/local/read_alignment_dna'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/targeted.nf:25:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/oncoanalyser/subworkflows/local/read_alignment_rna/main.nf'

  ```nextflow
  include { READ_ALIGNMENT_RNA       } from '../subworkflows/local/read_alignment_rna'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/targeted.nf:137:9`: `READ_ALIGNMENT_DNA` is not defined

  ```nextflow
          READ_ALIGNMENT_DNA(
          ^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/targeted.nf:145:9`: `READ_ALIGNMENT_RNA` is not defined

  ```nextflow
          READ_ALIGNMENT_RNA(
          ^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/targeted.nf:151:61`: `READ_ALIGNMENT_DNA` is not defined

  ```nextflow
          ch_align_dna_tumor_out = ch_align_dna_tumor_out.mix(READ_ALIGNMENT_DNA.out.tumor)
                                                              ^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/targeted.nf:152:63`: `READ_ALIGNMENT_DNA` is not defined

  ```nextflow
          ch_align_dna_normal_out = ch_align_dna_normal_out.mix(READ_ALIGNMENT_DNA.out.normal)
                                                                ^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/targeted.nf:153:61`: `READ_ALIGNMENT_DNA` is not defined

  ```nextflow
          ch_align_dna_donor_out = ch_align_dna_donor_out.mix(READ_ALIGNMENT_DNA.out.donor)
                                                              ^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/targeted.nf:155:61`: `READ_ALIGNMENT_RNA` is not defined

  ```nextflow
          ch_align_rna_tumor_out = ch_align_rna_tumor_out.mix(READ_ALIGNMENT_RNA.out.tumor)
                                                              ^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/wgts.nf:27:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/oncoanalyser/subworkflows/local/read_alignment_dna/main.nf'

  ```nextflow
  include { READ_ALIGNMENT_DNA    } from '../subworkflows/local/read_alignment_dna'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/wgts.nf:28:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/oncoanalyser/subworkflows/local/read_alignment_rna/main.nf'

  ```nextflow
  include { READ_ALIGNMENT_RNA    } from '../subworkflows/local/read_alignment_rna'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/wgts.nf:108:9`: `READ_ALIGNMENT_DNA` is not defined

  ```nextflow
          READ_ALIGNMENT_DNA(
          ^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/wgts.nf:116:9`: `READ_ALIGNMENT_RNA` is not defined

  ```nextflow
          READ_ALIGNMENT_RNA(
          ^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/wgts.nf:122:61`: `READ_ALIGNMENT_DNA` is not defined

  ```nextflow
          ch_align_dna_tumor_out = ch_align_dna_tumor_out.mix(READ_ALIGNMENT_DNA.out.tumor)
                                                              ^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/wgts.nf:123:63`: `READ_ALIGNMENT_DNA` is not defined

  ```nextflow
          ch_align_dna_normal_out = ch_align_dna_normal_out.mix(READ_ALIGNMENT_DNA.out.normal)
                                                                ^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/wgts.nf:124:61`: `READ_ALIGNMENT_DNA` is not defined

  ```nextflow
          ch_align_dna_donor_out = ch_align_dna_donor_out.mix(READ_ALIGNMENT_DNA.out.donor)
                                                              ^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/wgts.nf:126:61`: `READ_ALIGNMENT_RNA` is not defined

  ```nextflow
          ch_align_rna_tumor_out = ch_align_rna_tumor_out.mix(READ_ALIGNMENT_RNA.out.tumor)
                                                              ^^^^^^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `subworkflows/local/amber_profiling/main.nf:47:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx ->
                                     ^^^^^^^^^
  ```

- Warning: `subworkflows/local/amber_profiling/main.nf:47:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx ->
                                                            ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/amber_profiling/main.nf:47:71`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx ->
                                                                        ^^^^^^^^^
  ```

- Warning: `subworkflows/local/amber_profiling/main.nf:47:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx ->
                                                                                   ^^^^^^^^^
  ```

- Warning: `subworkflows/local/bamtools_metrics/main.nf:34:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, aln, idx ->
                               ^^^
  ```

- Warning: `subworkflows/local/bamtools_metrics/main.nf:51:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, aln, idx ->
                               ^^^
  ```

- Warning: `subworkflows/local/bamtools_metrics/main.nf:89:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta_bamtools, bamtools_dir ->
                                   ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/cider_calling/main.nf:10:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_inputs          // channel: [mandatory] [ meta ]
      ^^^^^^^^^
  ```

- Warning: `subworkflows/local/cider_calling/main.nf:33:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, aln, idx ->
                               ^^^
  ```

- Warning: `subworkflows/local/cider_calling/main.nf:49:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, aln, idx ->
                               ^^^
  ```

- Warning: `subworkflows/local/cobalt_profiling/main.nf:42:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx ->
                                     ^^^^^^^^^
  ```

- Warning: `subworkflows/local/cobalt_profiling/main.nf:42:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx ->
                                                            ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/cuppa_prediction/main.nf:40:70`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, isofox_dir, purple_dir, linx_annotation_dir, virusinterpreter_dir ->
                                                                       ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/esvee_calling/main.nf:50:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx ->
                                                            ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/isofox_quantification/main.nf:43:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx ->
                                     ^^^^^^^^^
  ```

- Warning: `subworkflows/local/lilac_calling/main.nf:56:41`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, normal_dna_aln, normal_dna_idx, tumor_dna_aln, tumor_dna_idx, tumor_rna_aln, tumor_rna_idx, purple_dir ->
                                          ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/lilac_calling/main.nf:56:72`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, normal_dna_aln, normal_dna_idx, tumor_dna_aln, tumor_dna_idx, tumor_rna_aln, tumor_rna_idx, purple_dir ->
                                                                         ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/lilac_calling/main.nf:56:87`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, normal_dna_aln, normal_dna_idx, tumor_dna_aln, tumor_dna_idx, tumor_rna_aln, tumor_rna_idx, purple_dir ->
                                                                                        ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/lilac_calling/main.nf:56:102`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, normal_dna_aln, normal_dna_idx, tumor_dna_aln, tumor_dna_idx, tumor_rna_aln, tumor_rna_idx, purple_dir ->
                                                                                                       ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/lilac_calling/main.nf:56:117`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, normal_dna_aln, normal_dna_idx, tumor_dna_aln, tumor_dna_idx, tumor_rna_aln, tumor_rna_idx, purple_dir ->
                                                                                                                      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/linx_annotation/main.nf:93:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, purple_dir ->
                          ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/linx_plotting/main.nf:44:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, linx_annotations_dir, amber_dir, cobalt_dir, purple_dir ->
                                                ^^^^^^^^^
  ```

- Warning: `subworkflows/local/linx_plotting/main.nf:44:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, linx_annotations_dir, amber_dir, cobalt_dir, purple_dir ->
                                                           ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/linx_plotting/main.nf:44:70`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, linx_annotations_dir, amber_dir, cobalt_dir, purple_dir ->
                                                                       ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/neo_prediction/main.nf:113:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, neo_finder_dir, tumor_rna_aln, tumor_rna_idx ->
                          ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/neo_prediction/main.nf:113:41`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, neo_finder_dir, tumor_rna_aln, tumor_rna_idx ->
                                          ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/neo_prediction/main.nf:113:56`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, neo_finder_dir, tumor_rna_aln, tumor_rna_idx ->
                                                         ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/neo_prediction/main.nf:191:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, isofox_dir, purple_dir, sage_append_dir_somatic, lilac_dir, neo_finder_dir, annotated_fusions ->
                          ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/neo_prediction/main.nf:191:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, isofox_dir, purple_dir, sage_append_dir_somatic, lilac_dir, neo_finder_dir, annotated_fusions ->
                                                  ^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/neo_prediction/main.nf:191:101`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, isofox_dir, purple_dir, sage_append_dir_somatic, lilac_dir, neo_finder_dir, annotated_fusions ->
                                                                                                      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/pave_annotation/main.nf:48:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, sage_vcf, sage_tbi ->
                                    ^^^^^^^^
  ```

- Warning: `subworkflows/local/pave_annotation/main.nf:101:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, sage_vcf, sage_tbi ->
                                    ^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_reference/main.nf:229:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .filter { meta, dir -> meta.topic_key == params.ref_data_panel_data_path }
                                  ^^^
  ```

- Warning: `subworkflows/local/prepare_reference/main.nf:230:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .map { meta, dir -> dir }
                         ^^^^
  ```

- Warning: `subworkflows/local/purple_calling/main.nf:58:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, amber_dir, cobalt_dir, esvee_dir, pave_somatic_dir, pave_germline_dir, redux_tsvs_tumor ->
                                                 ^^^^^^^^^
  ```

- Warning: `subworkflows/local/purple_calling/main.nf:58:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, amber_dir, cobalt_dir, esvee_dir, pave_somatic_dir, pave_germline_dir, redux_tsvs_tumor ->
                                                            ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/purple_calling/main.nf:58:77`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, amber_dir, cobalt_dir, esvee_dir, pave_somatic_dir, pave_germline_dir, redux_tsvs_tumor ->
                                                                              ^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/purple_calling/main.nf:58:96`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, amber_dir, cobalt_dir, esvee_dir, pave_somatic_dir, pave_germline_dir, redux_tsvs_tumor ->
                                                                                                 ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/qsee_metrics/main.nf:60:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, redux_tsvs_tumor, redux_tsvs_normal, bamtools_dir_tumor, bamtools_dir_normal, cobalt_dir, esvee_dir, purple_dir ->
                          ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/qsee_metrics/main.nf:60:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, redux_tsvs_tumor, redux_tsvs_normal, bamtools_dir_tumor, bamtools_dir_normal, cobalt_dir, esvee_dir, purple_dir ->
                                            ^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/qsee_metrics/main.nf:60:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, redux_tsvs_tumor, redux_tsvs_normal, bamtools_dir_tumor, bamtools_dir_normal, cobalt_dir, esvee_dir, purple_dir ->
                                                                                   ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/qsee_metrics/main.nf:60:103`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, redux_tsvs_tumor, redux_tsvs_normal, bamtools_dir_tumor, bamtools_dir_normal, cobalt_dir, esvee_dir, purple_dir ->
                                                                                                        ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/qsee_metrics/main.nf:60:115`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, redux_tsvs_tumor, redux_tsvs_normal, bamtools_dir_tumor, bamtools_dir_normal, cobalt_dir, esvee_dir, purple_dir ->
                                                                                                                    ^^^^^^^^^
  ```

- Warning: `subworkflows/local/read_umi_processing/main.nf:101:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch { meta_fastq, fastq_fwd, fastq_rev ->
                                    ^^^^^^^^^
  ```

- Warning: `subworkflows/local/read_umi_processing/main.nf:101:46`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch { meta_fastq, fastq_fwd, fastq_rev ->
                                               ^^^^^^^^^
  ```

- Warning: `subworkflows/local/read_umi_processing/main.nf:141:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch { meta_fastq, fastq_fwd, fastq_rev ->
                                    ^^^^^^^^^
  ```

- Warning: `subworkflows/local/read_umi_processing/main.nf:141:46`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch { meta_fastq, fastq_fwd, fastq_rev ->
                                               ^^^^^^^^^
  ```

- Warning: `subworkflows/local/read_umi_processing/main.nf:184:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta_fastq, fastq_info, fastq_fwd, fastq_rev ->
                                ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/read_umi_processing/main.nf:184:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta_fastq, fastq_info, fastq_fwd, fastq_rev ->
                                            ^^^^^^^^^
  ```

- Warning: `subworkflows/local/read_umi_processing/main.nf:184:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta_fastq, fastq_info, fastq_fwd, fastq_rev ->
                                                       ^^^^^^^^^
  ```

- Warning: `subworkflows/local/redux_processing/main.nf:43:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, alns, idxs ->
                                ^^^^
  ```

- Warning: `subworkflows/local/redux_processing/main.nf:58:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, alns, idxs ->
                                ^^^^
  ```

- Warning: `subworkflows/local/redux_processing/main.nf:73:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, alns, idxs ->
                                ^^^^
  ```

- Warning: `subworkflows/local/redux_processing/main.nf:124:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta_redux, redux_dir ->
                                ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_append/main.nf:59:52`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, purple_dir, tumor_dna_aln, tumor_dna_idx, redux_tsvs_tumor, tumor_rna_aln, tumor_rna_idx ->
                                                     ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_append/main.nf:59:67`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, purple_dir, tumor_dna_aln, tumor_dna_idx, redux_tsvs_tumor, tumor_rna_aln, tumor_rna_idx ->
                                                                    ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_append/main.nf:59:100`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, purple_dir, tumor_dna_aln, tumor_dna_idx, redux_tsvs_tumor, tumor_rna_aln, tumor_rna_idx ->
                                                                                                     ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_append/main.nf:73:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, purple_dir, tumor_dna_aln, tumor_dna_idx, redux_tsvs_tumor, tumor_rna_aln, tumor_rna_idx ->
                                      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_append/main.nf:73:52`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, purple_dir, tumor_dna_aln, tumor_dna_idx, redux_tsvs_tumor, tumor_rna_aln, tumor_rna_idx ->
                                                     ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_append/main.nf:73:67`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, purple_dir, tumor_dna_aln, tumor_dna_idx, redux_tsvs_tumor, tumor_rna_aln, tumor_rna_idx ->
                                                                    ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_append/main.nf:73:85`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, purple_dir, tumor_dna_aln, tumor_dna_idx, redux_tsvs_tumor, tumor_rna_aln, tumor_rna_idx ->
                                                                                      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_append/main.nf:73:100`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, purple_dir, tumor_dna_aln, tumor_dna_idx, redux_tsvs_tumor, tumor_rna_aln, tumor_rna_idx ->
                                                                                                     ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_append/main.nf:135:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, purple_dir, tumor_dna_aln, tumor_dna_idx, redux_tsvs_tumor, tumor_rna_aln, tumor_rna_idx ->
                                      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_append/main.nf:135:52`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, purple_dir, tumor_dna_aln, tumor_dna_idx, redux_tsvs_tumor, tumor_rna_aln, tumor_rna_idx ->
                                                     ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_append/main.nf:135:67`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, purple_dir, tumor_dna_aln, tumor_dna_idx, redux_tsvs_tumor, tumor_rna_aln, tumor_rna_idx ->
                                                                    ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_append/main.nf:135:85`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, purple_dir, tumor_dna_aln, tumor_dna_idx, redux_tsvs_tumor, tumor_rna_aln, tumor_rna_idx ->
                                                                                      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_append/main.nf:135:100`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, purple_dir, tumor_dna_aln, tumor_dna_idx, redux_tsvs_tumor, tumor_rna_aln, tumor_rna_idx ->
                                                                                                     ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:25:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      segment_mappability          // channel: [mandatory] /path/to/segment_mappability
      ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:63:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx, redux_tsvs ->
                                     ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:63:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx, redux_tsvs ->
                                                ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:63:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx, redux_tsvs ->
                                                            ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:63:71`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx, redux_tsvs ->
                                                                        ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:63:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx, redux_tsvs ->
                                                                                   ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:63:93`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx, redux_tsvs ->
                                                                                              ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:76:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx, redux_tsvs ->
                                     ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:76:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx, redux_tsvs ->
                                                            ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:76:71`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx, redux_tsvs ->
                                                                        ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:76:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx, redux_tsvs ->
                                                                                   ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:76:93`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx, redux_tsvs ->
                                                                                              ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:122:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx, redux_tsvs ->
                                     ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:122:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx, redux_tsvs ->
                                                ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:122:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx, redux_tsvs ->
                                                            ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:122:71`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx, redux_tsvs ->
                                                                        ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:122:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx, redux_tsvs ->
                                                                                   ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_calling/main.nf:122:93`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx, redux_tsvs ->
                                                                                              ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_plotting/main.nf:67:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx, redux_tsvs, purple_dir ->
                                     ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_plotting/main.nf:67:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx, redux_tsvs, purple_dir ->
                                                ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_plotting/main.nf:67:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx, redux_tsvs, purple_dir ->
                                                            ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_plotting/main.nf:67:71`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx, redux_tsvs, purple_dir ->
                                                                        ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_plotting/main.nf:67:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx, redux_tsvs, purple_dir ->
                                                                                   ^^^^^^^^^
  ```

- Warning: `subworkflows/local/sage_plotting/main.nf:67:93`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx, donor_aln, donor_idx, redux_tsvs, purple_dir ->
                                                                                              ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/teal_characterisation/main.nf:47:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx ->
                                     ^^^^^^^^^
  ```

- Warning: `subworkflows/local/teal_characterisation/main.nf:47:59`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx, normal_aln, normal_idx ->
                                                            ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/teal_characterisation/main.nf:127:41`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, teal_bam_tumor, teal_bai_tumor, teal_bam_normal, teal_bai_normal, bamtools_dir_tumor, bamtools_dir_normal, cobalt_dir, purple_dir ->
                                          ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/teal_characterisation/main.nf:127:74`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, teal_bam_tumor, teal_bai_tumor, teal_bam_normal, teal_bai_normal, bamtools_dir_tumor, bamtools_dir_normal, cobalt_dir, purple_dir ->
                                                                           ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_oncoanalyser_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/virusbreakend_calling/main.nf:45:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, tumor_aln, tumor_idx ->
                                     ^^^^^^^^^
  ```

- Warning: `subworkflows/local/wisp_analysis/main.nf:10:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_inputs                  // channel: [mandatory] [ meta ]
      ^^^^^^^^^
  ```

- Warning: `subworkflows/local/wisp_analysis/main.nf:54:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, primary_purple_dir, primary_amber_dir, primary_normal_aln, longitudinal_redux_dir, longitudinal_amber_dir, longitudinal_cobalt_dir, longitudinal_sage_append_dir ->
                                              ^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/wisp_analysis/main.nf:54:64`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, primary_purple_dir, primary_amber_dir, primary_normal_aln, longitudinal_redux_dir, longitudinal_amber_dir, longitudinal_cobalt_dir, longitudinal_sage_append_dir ->
                                                                 ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/wisp_analysis/main.nf:54:84`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, primary_purple_dir, primary_amber_dir, primary_normal_aln, longitudinal_redux_dir, longitudinal_amber_dir, longitudinal_cobalt_dir, longitudinal_sage_append_dir ->
                                                                                     ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/wisp_analysis/main.nf:54:108`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, primary_purple_dir, primary_amber_dir, primary_normal_aln, longitudinal_redux_dir, longitudinal_amber_dir, longitudinal_cobalt_dir, longitudinal_sage_append_dir ->
                                                                                                             ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/targeted.nf:96:5`: Variable was declared but not used

  ```nextflow
      ch_align_rna_qc_tumor_out = channel.empty()
      ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/wgts.nf:100:5`: Variable was declared but not used

  ```nextflow
      ch_align_rna_qc_tumor_out = channel.empty()
      ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```
