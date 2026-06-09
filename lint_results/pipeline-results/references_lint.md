# Nextflow lint results

- Generated: 2026-06-09T00:38:22.637835720Z
- Nextflow version: 26.04.3
- Summary: 48 warnings

## :warning: Warnings

- Warning: `modules/local/gawk/main.nf:29:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      suffix = task.ext.suffix ?: "${input.collect { it.getExtension() }.get(0)}"
                                                     ^^
  ```

- Warning: `modules/local/gawk/main.nf:32:34`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      lst_gz = input.findResults { it.getExtension().endsWith("gz") ? it.toString() : null }
                                   ^^
  ```

- Warning: `modules/local/gawk/main.nf:32:69`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      lst_gz = input.findResults { it.getExtension().endsWith("gz") ? it.toString() : null }
                                                                      ^^
  ```

- Warning: `modules/local/gawk/main.nf:34:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      input_cmd = input.collect { it.toString() - ~/\.gz$/ }.join(" ")
                                  ^^
  ```

- Warning: `modules/local/gawk/main.nf:37:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      cleanup = lst_gz ? "rm ${lst_gz.collect { it - ~/\.gz$/ }.join(" ")}" : ""
                                                ^^
  ```

- Warning: `modules/local/gawk/main.nf:40:16`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          assert it.name != "${prefix}.${suffix}" : "Input and output names are the same, set prefix in module configuration to disambiguate!"
                 ^^
  ```

- Warning: `modules/local/gffread/main.nf:25:91`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def extension = args.contains("-T") ? 'gtf' : (['-w', '-x', '-y'].any { args.contains(it) } ? 'fasta' : 'gff3')
                                                                                            ^^
  ```

- Warning: `modules/local/gffread/main.nf:45:91`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def extension = args.contains("-T") ? 'gtf' : (['-w', '-x', '-y'].any { args.contains(it) } ? 'fasta' : 'gff3')
                                                                                            ^^
  ```

- Warning: `modules/local/rsem/preparereference/main.nf:27:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          args_list.removeIf { it.contains('--star') }
                               ^^
  ```

- Warning: `subworkflows/local/datasheet_to_channel/main.nf:20:5`: Variable was declared but not used

  ```nextflow
      ascat_alleles = ascat_alleles_branch.file
      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/datasheet_to_channel/main.nf:29:5`: Variable was declared but not used

  ```nextflow
      ascat_loci = ascat_loci_branch.file
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/datasheet_to_channel/main.nf:38:5`: Variable was declared but not used

  ```nextflow
      ascat_loci_gc = ascat_loci_gc_branch.file
      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/datasheet_to_channel/main.nf:47:5`: Variable was declared but not used

  ```nextflow
      ascat_loci_rt = ascat_loci_rt_branch.file
      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/datasheet_to_channel/main.nf:56:5`: Variable was declared but not used

  ```nextflow
      chr_dir = chr_dir_branch.file
      ^^^^^^^
  ```

- Warning: `subworkflows/local/datasheet_to_channel/main.nf:65:5`: Variable was declared but not used

  ```nextflow
      intervals_bed = intervals_bed_branch.file
      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/datasheet_to_channel/main.nf:90:5`: Variable was declared but not used

  ```nextflow
      fasta = fasta_branch.file
      ^^^^^
  ```

- Warning: `subworkflows/local/datasheet_to_channel/main.nf:99:5`: Variable was declared but not used

  ```nextflow
      fasta_dict = fasta_dict_branch.file
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/datasheet_to_channel/main.nf:111:5`: Variable was declared but not used

  ```nextflow
      fasta_fai = fasta_fai_branch.file
      ^^^^^^^^^
  ```

- Warning: `subworkflows/local/datasheet_to_channel/main.nf:120:5`: Variable was declared but not used

  ```nextflow
      fasta_sizes = fasta_sizes_branch.file
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/datasheet_to_channel/main.nf:133:5`: Variable was declared but not used

  ```nextflow
      gff = gff_branch.file
      ^^^
  ```

- Warning: `subworkflows/local/datasheet_to_channel/main.nf:145:5`: Variable was declared but not used

  ```nextflow
      gtf = gtf_branch.file
      ^^^
  ```

- Warning: `subworkflows/local/datasheet_to_channel/main.nf:154:5`: Variable was declared but not used

  ```nextflow
      splice_sites = splice_sites_branch.file
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/datasheet_to_channel/main.nf:170:5`: Variable was declared but not used

  ```nextflow
      transcript_fasta = transcript_fasta_branch.file
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/datasheet_to_channel/main.nf:235:5`: Variable was declared but not used

  ```nextflow
      vcf = channel.empty().mix(dbsnp_branch.file, germline_resource_branch.file, known_indels_branch.file, known_snps_branch.file, pon_branch.file).transpose()
      ^^^
  ```

- Warning: `subworkflows/local/prepare_genome_dnaseq/main.nf:28:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      bwamem1_index = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome_dnaseq/main.nf:29:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      bwamem2_index = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome_dnaseq/main.nf:30:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      dragmap_hashmap = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome_dnaseq/main.nf:31:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      fasta_dict = Channel.empty()
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome_dnaseq/main.nf:32:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      intervals_bed = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome_dnaseq/main.nf:33:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      msisensorpro_list = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome_dnaseq/main.nf:34:14`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_gz = Channel.empty()
               ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome_dnaseq/main.nf:35:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_tbi = Channel.empty()
                ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome_dnaseq/main.nf:36:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      snapaligner_index = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome_rnaseq/main.nf:34:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      bowtie1_index = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome_rnaseq/main.nf:35:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      bowtie2_index = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome_rnaseq/main.nf:36:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      hisat2_index = Channel.empty()
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome_rnaseq/main.nf:37:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      kallisto_index = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome_rnaseq/main.nf:38:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      rsem_index = Channel.empty()
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome_rnaseq/main.nf:39:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      salmon_index = Channel.empty()
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome_rnaseq/main.nf:40:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      star_index = Channel.empty()
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome_rnaseq/main.nf:41:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      fasta_sizes = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_references_pipeline/main.nf:143:5`: Variable was declared but not used

  ```nextflow
      references = channel.fromList(
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_references_pipeline/main.nf:151:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      references
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_references/main.nf:20:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      references = Channel.fromList(
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_references/main.nf:28:5`: Variable was declared but not used

  ```nextflow
      references_file = get_references_file(references, param_file, attribute_file)
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_references/main.nf:29:5`: Variable was declared but not used

  ```nextflow
      references_value = get_references_value(references, param_value, attribute_value)
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/references.nf:86:5`: Variable was declared but not used

  ```nextflow
      references = channel.empty()
      ^^^^^^^^^^
  ```

- Warning: `workflows/references.nf:117:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      references // channel: [meta, *]
      ^^^^^^^^^^
  ```
