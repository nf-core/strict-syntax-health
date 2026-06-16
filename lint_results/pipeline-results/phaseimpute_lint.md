# Nextflow lint results

- Generated: 2026-06-16T19:35:41.201323323Z
- Nextflow version: 26.04.3
- Summary: 19 warnings

## :warning: Warnings

- Warning: `main.nf:134:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = PHASEIMPUTE.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_chr_rename_samtools/main.nf:36:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      bam_renamed    = ch_bam_renamed        // [ [id], bam, index ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_extract_region_samtools/main.nf:50:9`: Emit name should be omitted when there is only one emit

  ```nextflow
          bam_region = ch_bam_region_all // channel: [ [id, chr], bam, index ]
          ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:49:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      ch_fasta_fai_gzi = ch_fasta_fai_gzi
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_chr_rename_bcftools/main.nf:54:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf_renamed    = ch_vcf_renamed        // [ [id], vcf, csi ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_normalize_bcftools/main.nf:49:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf_tbi        = ch_vcf_tbi                     // channel: [ [id, chr], vcf, tbi ]
      ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_sites_extract_bcftools/main.nf:35:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      posfile       = ch_posfile          // channel: [ [id, chr], vcf, csi, hap, legend, posfile ]
      ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_split_bcftools/main.nf:23:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf_tbi        = ch_vcf_tbi_samples   // channel: [ [id, chr, tools], vcf, index ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_impute_quilt/main.nf:76:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf_index = ch_vcf_index // channel:   [ [id, chr], vcf, tbi ]
      ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_impute_quilt2/main.nf:75:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf_index = ch_vcf_index // channel: [ meta, vcf, tbi/csi ]
      ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_impute_stitch/main.nf:86:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf_index = ch_vcf_index // channel:   [ [id, chr], vcf, tbi ]
      ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_subsampledepth_samtools/main.nf:51:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      bam_subsampled    = ch_bam_subsampled             // channel: [ val(meta), path(bam), path(csi) ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
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

- Warning: `subworkflows/nf-core/vcf_impute_beagle5/main.nf:119:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf_index = ch_vcf_index // channel: [ [id, chr, tools], vcf, index ]
      ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/vcf_impute_minimac4/main.nf:90:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf_index = ch_vcf_index // channel: [ [id, panel, chr], vcf, index ]
      ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/chrcheck/main.nf:73:9`: Emit name should be omitted when there is only one emit

  ```nextflow
          output   = ch_output             // [ [id], file, index ]
          ^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/phaseimpute/main.nf:820:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = MULTIQC.out.report.map { _meta, report -> [report] }.toList() // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```
