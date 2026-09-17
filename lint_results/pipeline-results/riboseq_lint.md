# Nextflow lint results

- Generated: 2026-09-17T00:21:55.334262940Z
- Nextflow version: 26.08.0-edge
- Summary: 11 warnings

## :warning: Warnings

- Warning: `modules/local/dte_counts_prep/main.nf:22:5`: Variable was declared but not used

  ```nextflow
      args   = task.ext.args ?: ''
      ^^^^
  ```

- Warning: `modules/local/orf_count_matrix/main.nf:22:5`: Variable was declared but not used

  ```nextflow
      sample_ids_b64 = groovy.json.JsonOutput.toJson(sample_ids).bytes.encodeBase64().toString()
      ^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/custom/bed12codonpositions/main.nf:22:5`: Variable was declared but not used

  ```nextflow
      args   = task.ext.args ?: ''
      ^^^^
  ```

- Warning: `modules/nf-core/custom/orfcollapse/main.nf:29:5`: Variable was declared but not used

  ```nextflow
      args   = task.ext.args ?: ''
      ^^^^
  ```

- Warning: `modules/nf-core/custom/orfmerge/main.nf:28:5`: Variable was declared but not used

  ```nextflow
      args   = task.ext.args ?: ''
      ^^^^
  ```

- Warning: `modules/nf-core/custom/orfnormalise/main.nf:24:5`: Variable was declared but not used

  ```nextflow
      sample_id = meta.id ?: 'unknown'
      ^^^^^^^^^
  ```

- Warning: `modules/nf-core/custom/orfnormalise/main.nf:25:5`: Variable was declared but not used

  ```nextflow
      args      = task.ext.args ?: ''
      ^^^^
  ```

- Warning: `modules/nf-core/rpbp/getperiodiclengthsoffsets/main.nf:21:5`: Variable was declared but not used

  ```nextflow
      task_ext_args = task.ext.args ?: ''
      ^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/rpbp/preparegenome/main.nf:23:5`: Variable was declared but not used

  ```nextflow
      task_ext_args = task.ext.args ?: ''
      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/orftable_fasta_gtf_buildorfcatalogue/main.nf:49:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it.size() > 0 }
                    ^^
  ```

- Warning: `subworkflows/nf-core/orftable_fasta_gtf_buildorfcatalogue/main.nf:55:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it.size() > 0 }
                    ^^
  ```
