# Nextflow lint results

- Generated: 2026-02-19T00:25:12.765973+00:00
- Nextflow version: 26.01.1-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/nf-core/fastq_preprocess_seqkit/main.nf:63:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              def clean_meta = meta.findAll { key, value -> key != 'strandness' }
                                                   ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_preprocess_seqkit/main.nf:71:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def sorted_files = files.flatten().sort { it.name }
                                                            ^^^^^^^^^
  ```
