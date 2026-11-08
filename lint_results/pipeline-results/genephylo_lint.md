# Nextflow lint results

- Generated: 2026-11-07T00:11:12.902368238Z
- Nextflow version: 26.10.5
- Summary: 1 error, 18 warnings

## :x: Errors

- Error: `workflows/genephylo.nf:125:2`: Incorrect number of call arguments, expected 3 but received 1

  ```nextflow
  	TD2_LONGORFS(ch_orf_in)
   ^^^^^^^^^^^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `modules/local/blast_extract.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/ete_taxdb.nf:16:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/blast/blastdbcmd/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/blast/blastn/main.nf:24:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/blast/makeblastdb/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/blast/tblastn/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/blast/updateblastdb/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/fasttree/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/iqtree/main.nf:54:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/mafft/align/main.nf:27:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/seqkit/rmdup/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/td2/longorfs/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/td2/predict/main.nf:24:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:15:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input_workflow      // workflow: the workflow object used by nf-schema to get metadata from the workflow
      ^^^^^^^^^^^^^^
  ```

- Warning: `workflows/genephylo.nf:86:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
  	ch_blast_in = ch_samplesheet.map { meta, fasta, tree -> tuple(meta, file(fasta)) }
                                                   ^^^^
  ```

- Warning: `workflows/genephylo.nf:138:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def cds_file = files.find { it.name.endsWith('.TD2.cds') }
                                      ^^
  ```

- Warning: `workflows/genephylo.nf:150:2`: Variable was declared but not used

  ```nextflow
  	ch_mafft_out = MAFFT_ALIGN.out.fas
   ^^^^^^^^^^^^
  ```

- Warning: `workflows/genephylo.nf:193:9`: Variable was declared but not used

  ```nextflow
      def ch_collated_versions = softwareVersionsToYAML(ch_versions.mix(topic_versions.versions_file))
          ^^^^^^^^^^^^^^^^^^^^
  ```
