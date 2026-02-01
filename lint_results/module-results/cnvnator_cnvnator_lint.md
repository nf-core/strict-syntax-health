# Nextflow lint results

- Generated: 2026-02-01T00:22:15.887657+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 error

## :x: Errors

- Error: `modules/nf-core/cnvnator/cnvnator/main.nf:53:9`: `calls_cmd` is already declared

  ```nextflow
      def calls_cmd = args.contains("-call") ? "touch ${prefix}.tab" : ''
          ^^^^^^^^^^
  ```
