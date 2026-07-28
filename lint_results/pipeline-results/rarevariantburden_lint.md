# Nextflow lint results

- Generated: 2026-07-28T00:33:24.539602533Z
- Nextflow version: 26.07.0-edge
- Summary: 22 warnings

## :warning: Warnings

- Warning: `subworkflows/local/utils_nfcore_rarevariantburden_pipeline/main.nf:31:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:101:98`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      return ch_versions.unique().map { version -> processVersionsFromYAML(version) }.unique().mix(Channel.of(workflowVersionToYAML()))
                                                                                                   ^^^^^^^
  ```

- Warning: `workflows/rarevariantburden.nf:40:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      caseJointVCF // caseJointVCF read in from --caseJointVCF
      ^^^^^^^^^^^^
  ```

- Warning: `workflows/rarevariantburden.nf:41:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      caseSample // caseSample read in from --caseSample
      ^^^^^^^^^^
  ```

- Warning: `workflows/rarevariantburden.nf:50:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      activeProfiles = workflow.profile.tokenize(',').collect { it.trim() }
                                                                ^^
  ```

- Warning: `workflows/rarevariantburden.nf:51:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      useCondaCoCoRV = activeProfiles.any { it == 'conda' || it == 'mamba' }
                                            ^^
  ```

- Warning: `workflows/rarevariantburden.nf:51:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      useCondaCoCoRV = activeProfiles.any { it == 'conda' || it == 'mamba' }
                                                             ^^
  ```

- Warning: `workflows/rarevariantburden.nf:54:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          BUILD_COCORV(Channel.fromPath("${params.CoCoRVFolder}/CoCoRV", checkIfExists: true))
                       ^^^^^^^
  ```

- Warning: `workflows/rarevariantburden.nf:57:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          cocorvRlibChannel = Channel.value([])
                              ^^^^^^^
  ```

- Warning: `workflows/rarevariantburden.nf:62:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          intersectChannel = Channel.value(params.controlBed)
                             ^^^^^^^
  ```

- Warning: `workflows/rarevariantburden.nf:70:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      chromChannel = Channel.fromList(Arrays.asList(chromosomes))
                     ^^^^^^^
  ```

- Warning: `workflows/rarevariantburden.nf:81:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          caseVCF_ch = Channel
                       ^^^^^^^
  ```

- Warning: `workflows/rarevariantburden.nf:91:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              normalizeQCChannel = Channel
                                   ^^^^^^^
  ```

- Warning: `workflows/rarevariantburden.nf:117:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          annotateChannel = Channel
                            ^^^^^^^
  ```

- Warning: `workflows/rarevariantburden.nf:133:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          caseGenotypeGDSChannel = Channel
                                   ^^^^^^^
  ```

- Warning: `workflows/rarevariantburden.nf:138:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          caseAnnotationGDSChannel = Channel
                                     ^^^^^^^
  ```

- Warning: `workflows/rarevariantburden.nf:163:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          populationChannel = Channel.value(params.casePopulation)
                              ^^^^^^^
  ```

- Warning: `workflows/rarevariantburden.nf:169:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      controlGenotypeGDSChannel = Channel
                                  ^^^^^^^
  ```

- Warning: `workflows/rarevariantburden.nf:173:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      controlAnnotationGDSChannel = Channel
                                    ^^^^^^^
  ```

- Warning: `workflows/rarevariantburden.nf:202:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      mergeCoCoRVResults(cocorvOutChannel.map{it[1]}.collect(), cocorvOutChannel.map{it[2]}.collect(),
                                              ^^
  ```

- Warning: `workflows/rarevariantburden.nf:202:84`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      mergeCoCoRVResults(cocorvOutChannel.map{it[1]}.collect(), cocorvOutChannel.map{it[2]}.collect(),
                                                                                     ^^
  ```

- Warning: `workflows/rarevariantburden.nf:203:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          cocorvOutChannel.map{it[3]}.collect())
                               ^^
  ```
