# Nextflow lint results

- Generated: 2026-07-23T00:32:17.564186382Z
- Nextflow version: 26.07.0-edge
- Summary: 8 errors, 26 warnings

## :x: Errors

- Error: `conf/test.config:21:1`: Variable declarations cannot be mixed with config statements

  ```nextflow
  def caseRoot = params.pipelines_testdata_base_path + "rarevariantburden/case"
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `conf/test.config:32:23`: `caseRoot` is not defined

  ```nextflow
      caseJointVCF = "${caseRoot}/samples.1KG.chr21-22.vcf.gz"
                        ^^^^^^^^
  ```

- Error: `conf/test.config:33:21`: `caseRoot` is not defined

  ```nextflow
      caseSample = "${caseRoot}/samples.txt"
                      ^^^^^^^^
  ```

- Error: `conf/test.config:49:35`: `caseRoot` is not defined

  ```nextflow
      caseAnnotatedVCFFileList = "${caseRoot}/annotationFiles.csv"
                                    ^^^^^^^^
  ```

- Error: `conf/test.config:51:36`: `caseRoot` is not defined

  ```nextflow
      caseAnnotationGDSFileList = "${caseRoot}/annotationGDSFiles.csv"
                                     ^^^^^^^^
  ```

- Error: `conf/test.config:53:34`: `caseRoot` is not defined

  ```nextflow
      caseGenotypeGDSFileList = "${caseRoot}/genotypeGDSFiles.csv"
                                   ^^^^^^^^
  ```

- Error: `conf/test.config:55:25`: `caseRoot` is not defined

  ```nextflow
      casePopulation = "${caseRoot}/casePopulation.txt"
                          ^^^^^^^^
  ```

- Error: `main.nf:104:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  workflow.onComplete {
  ^
  ```

## :warning: Warnings

- Warning: `main.nf:159:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          it.name.matches(pattern.replace('*', '.*'))
                          ^^
  ```

- Warning: `main.nf:161:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          it.copyTo("${destDir}/${it.name}")
                          ^^
  ```

- Warning: `main.nf:161:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          it.copyTo("${destDir}/${it.name}")
                                                  ^^
  ```

- Warning: `main.nf:162:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          log.info "✓ Copied ${it.name} to ${destDir}"
                                               ^^
  ```

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

- Warning: `workflows/rarevariantburden.nf:92:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              normalizeQCChannel = Channel
                                   ^^^^^^^
  ```

- Warning: `workflows/rarevariantburden.nf:119:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          annotateChannel = Channel
                            ^^^^^^^
  ```

- Warning: `workflows/rarevariantburden.nf:136:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          caseGenotypeGDSChannel = Channel
                                   ^^^^^^^
  ```

- Warning: `workflows/rarevariantburden.nf:142:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          caseAnnotationGDSChannel = Channel
                                     ^^^^^^^
  ```

- Warning: `workflows/rarevariantburden.nf:168:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          populationChannel = Channel.value(params.casePopulation)
                              ^^^^^^^
  ```

- Warning: `workflows/rarevariantburden.nf:174:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      controlGenotypeGDSChannel = Channel
                                  ^^^^^^^
  ```

- Warning: `workflows/rarevariantburden.nf:179:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      controlAnnotationGDSChannel = Channel
                                    ^^^^^^^
  ```

- Warning: `workflows/rarevariantburden.nf:209:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      mergeCoCoRVResults(cocorvOutChannel.map{it[1]}.collect(), cocorvOutChannel.map{it[2]}.collect(),
                                              ^^
  ```

- Warning: `workflows/rarevariantburden.nf:209:84`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      mergeCoCoRVResults(cocorvOutChannel.map{it[1]}.collect(), cocorvOutChannel.map{it[2]}.collect(),
                                                                                     ^^
  ```

- Warning: `workflows/rarevariantburden.nf:210:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          cocorvOutChannel.map{it[3]}.collect())
                               ^^
  ```
