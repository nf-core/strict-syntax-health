# Workflow outputs migration: meerpipe

- Generated: 2026-06-16T14:22:02.332784+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 9 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:16`](https://github.com/nf-core/meerpipe/blob/76b676212bdf0a9de91ac1497d237211a492f153/conf/modules.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:24`](https://github.com/nf-core/meerpipe/blob/76b676212bdf0a9de91ac1497d237211a492f153/conf/modules.config#L24)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/decimate.nf:7`](https://github.com/nf-core/meerpipe/blob/76b676212bdf0a9de91ac1497d237211a492f153/modules/local/decimate.nf#L7)

  ```nextflow
  publishDir "${params.outdir}/${meta.pulsar}/${meta.utc}/${meta.beam}/decimated", mode: 'copy', pattern: "${meta.pulsar}_${meta.utc}_{raw,zap}*t.ar"
  ```

- [`modules/local/generate_image_results.nf:7`](https://github.com/nf-core/meerpipe/blob/76b676212bdf0a9de91ac1497d237211a492f153/modules/local/generate_image_results.nf#L7)

  ```nextflow
  publishDir "${params.outdir}/${meta.pulsar}/${meta.utc}/${meta.beam}/images", mode: 'copy', pattern: "{c,t,r}*png"
  ```

- [`modules/local/generate_image_results.nf:8`](https://github.com/nf-core/meerpipe/blob/76b676212bdf0a9de91ac1497d237211a492f153/modules/local/generate_image_results.nf#L8)

  ```nextflow
  publishDir "${params.outdir}/${meta.pulsar}/${meta.utc}/${meta.beam}/scintillation", mode: 'copy', pattern: "*dynspec*"
  ```

- [`modules/local/generate_image_results.nf:9`](https://github.com/nf-core/meerpipe/blob/76b676212bdf0a9de91ac1497d237211a492f153/modules/local/generate_image_results.nf#L9)

  ```nextflow
  publishDir "${params.outdir}/${meta.pulsar}/${meta.utc}/${meta.beam}", mode: 'copy', pattern: "results.json"
  ```

- [`modules/local/generate_toas.nf:6`](https://github.com/nf-core/meerpipe/blob/76b676212bdf0a9de91ac1497d237211a492f153/modules/local/generate_toas.nf#L6)

  ```nextflow
  publishDir "${params.outdir}/${meta.pulsar}/${meta.utc}/${meta.beam}/timing/${meta.project_short}", mode: 'copy', pattern: "*.{tim,par,std}"
  ```

- [`modules/local/psradd_calibrate_clean.nf:7`](https://github.com/nf-core/meerpipe/blob/76b676212bdf0a9de91ac1497d237211a492f153/modules/local/psradd_calibrate_clean.nf#L7)

  ```nextflow
  publishDir "${params.outdir}/${meta.pulsar}/${meta.utc}/${meta.beam}", mode: params.publish_dir_mode, pattern: "${ template.baseName == "no_template" ? "*raw.ar" : "*zap.ar" }"
  ```

- [`modules/local/psradd_calibrate_clean.nf:39`](https://github.com/nf-core/meerpipe/blob/76b676212bdf0a9de91ac1497d237211a492f153/modules/local/psradd_calibrate_clean.nf#L39)

  ```nextflow
  # Grab obs.header to output it the publishDir
  ```
