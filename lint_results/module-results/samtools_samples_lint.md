# Nextflow lint results

- Generated: 2026-02-09T00:23:26.233578+00:00
- Nextflow version: 26.01.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/samtools/samples/main.nf:25:61`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def fasta_arg = fasta ? [fasta].flatten().collect { "-f $it" }.join(' ') : ''
                                                              ^^^^^^^^^^
  ```
