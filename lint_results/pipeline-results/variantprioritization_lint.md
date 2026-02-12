# Nextflow lint results

- Generated: 2026-02-12T00:23:54.453142066Z
- Nextflow version: 26.01.1-edge
- Summary: 5 errors

## :x: Errors

- Error: `subworkflows/local/utils_nfcore_variantprioritization_pipeline/main.nf:4:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import java.util.zip.GZIPInputStream
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/utils_nfcore_variantprioritization_pipeline/main.nf:5:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import groovy.transform.Field
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/utils_nfcore_variantprioritization_pipeline/main.nf:193:24`: `GZIPInputStream` is not defined

  ```nextflow
              def gzis = new GZIPInputStream(fis)
                         ^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/utils_nfcore_variantprioritization_pipeline/main.nf:217:43`: `GZIPInputStream` is not defined

  ```nextflow
          (vcf.toString().endsWith('.gz') ? new GZIPInputStream(vcf.newInputStream()) : vcf.newInputStream()).withReader { reader ->
                                            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/utils_nfcore_variantprioritization_pipeline/main.nf:237:17`: `GZIPInputStream` is not defined

  ```nextflow
                  new GZIPInputStream(fis).withReader { reader ->
                  ^^^^^^^^^^^^^^^^^^^^^^^^
  ```
