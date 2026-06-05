# Nextflow lint results

- Generated: 2026-06-05T00:42:11.579403129Z
- Nextflow version: 26.04.3
- Summary: 6 warnings

## :warning: Warnings

- Warning: `subworkflows/local/cnvkit_pon/main.nf:27:55`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_reads.bam.mix(SAMTOOLS_VIEW.out.bam).map { meta, bam -> [[id: 'panel'], bam] }.groupTuple().map { meta, bam -> [meta, [], [], bam, []] },
                                                        ^^^^
  ```

- Warning: `subworkflows/local/prepare_alignment/main.nf:43:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      reads_index = ch_reads_index // [ val(meta), path(bam|cram), path(bai|crai) ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_createpanelrefs_pipeline/main.nf:131:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      samplesheet = ch_samplesheet
      ^^^^^^^^^^^^^^^^^^^^^^^^^^
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

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:76:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```
