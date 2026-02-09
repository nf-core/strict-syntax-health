# Nextflow lint results

- Generated: 2026-02-09T00:23:26.269742+00:00
- Nextflow version: 26.01.0-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `modules/nf-core/wipertools/fastqgather/main.nf:23:35`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      fastq_string = fastq.collect{ it.name }.sort().join(" ")
                                    ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/wipertools/fastqgather/main.nf:26:21`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      if (fastq.any { it.name == "${prefix}.fastq.gz" }) {
                      ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/wipertools/fastqgather/main.nf:47:21`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      if (fastq.any { it.name == "${prefix}.fastq.gz" }) {
                      ^^^^^^^^^^
  ```
