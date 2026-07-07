# Nextflow lint results

- Generated: 2026-07-07T00:40:15.410703248Z
- Nextflow version: 26.06.0-edge
- Summary: 12 warnings

## :warning: Warnings

- Warning: `main.nf:54:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = VIRALMETAGENOME.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_vcf_consensus_bcftools/main.nf:72:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      consensus = BCFTOOLS_CONSENSUS.out.fasta // channel: [ val(meta), [ fasta ] ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/fasta_contig_preclust/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      ch_versions = channel.empty()
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/mmseqs_annotate/main.nf:18:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      tsv      = MMSEQS_EASYSEARCH.out.tsv // channel: [ val(meta), [ tsv ] ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/singleton_filtering/main.nf:25:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      filtered     = RENAME_FASTA_HEADER_SINGLETON.out.fasta  // channel: [ val(meta), [ fasta ] ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/unpack_db/main.nf:28:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      db       = ch_db_unpacked // channel: [ db ]
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralmetagenome_pipeline/tests/lazymap_test.nf:19:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      parsed          = Channel.value(parsed_map)
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralmetagenome_pipeline/tests/lazymap_test.nf:20:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      class_name      = Channel.value(parsed_map.getClass().name)
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralmetagenome_pipeline/tests/lazymap_test.nf:21:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      is_serializable = Channel.value(parsed_map instanceof java.io.Serializable)
                        ^^^^^^^
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
