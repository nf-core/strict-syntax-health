# Workflow outputs migration: rarevariantburden

- Generated: 2026-06-16T14:29:55.271371+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 18 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/rarevariantburden/blob/e9392c4294ecdd4f6f984b9c235eb220306455be/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/cocorv/main.nf:28`](https://github.com/nf-core/rarevariantburden/blob/e9392c4294ecdd4f6f984b9c235eb220306455be/modules/local/cocorv/main.nf#L28)

  ```nextflow
  publishDir "${params.outdir}", mode: 'copy'
  ```

- [`modules/local/cocorv/main.nf:49`](https://github.com/nf-core/rarevariantburden/blob/e9392c4294ecdd4f6f984b9c235eb220306455be/modules/local/cocorv/main.nf#L49)

  ```nextflow
  publishDir "${params.outdir}/vcf_vqsr_normalizedQC", mode: 'copy'
  ```

- [`modules/local/cocorv/main.nf:72`](https://github.com/nf-core/rarevariantburden/blob/e9392c4294ecdd4f6f984b9c235eb220306455be/modules/local/cocorv/main.nf#L72)

  ```nextflow
  publishDir "${params.outdir}/vcf_vqsr_normalizedQC", mode: 'copy'
  ```

- [`modules/local/cocorv/main.nf:92`](https://github.com/nf-core/rarevariantburden/blob/e9392c4294ecdd4f6f984b9c235eb220306455be/modules/local/cocorv/main.nf#L92)

  ```nextflow
  publishDir "${params.outdir}/annotation", mode: 'copy'
  ```

- [`modules/local/cocorv/main.nf:123`](https://github.com/nf-core/rarevariantburden/blob/e9392c4294ecdd4f6f984b9c235eb220306455be/modules/local/cocorv/main.nf#L123)

  ```nextflow
  publishDir "${params.outdir}/annotation", mode: 'copy'
  ```

- [`modules/local/cocorv/main.nf:191`](https://github.com/nf-core/rarevariantburden/blob/e9392c4294ecdd4f6f984b9c235eb220306455be/modules/local/cocorv/main.nf#L191)

  ```nextflow
  publishDir "${params.outdir}/annotation", mode: 'copy'
  ```

- [`modules/local/cocorv/main.nf:211`](https://github.com/nf-core/rarevariantburden/blob/e9392c4294ecdd4f6f984b9c235eb220306455be/modules/local/cocorv/main.nf#L211)

  ```nextflow
  publishDir "${params.outdir}/vcf_vqsr_normalizedQC", mode: 'copy'
  ```

- [`modules/local/cocorv/main.nf:234`](https://github.com/nf-core/rarevariantburden/blob/e9392c4294ecdd4f6f984b9c235eb220306455be/modules/local/cocorv/main.nf#L234)

  ```nextflow
  publishDir "${params.outdir}/annotation", mode: 'copy'
  ```

- [`modules/local/cocorv/main.nf:257`](https://github.com/nf-core/rarevariantburden/blob/e9392c4294ecdd4f6f984b9c235eb220306455be/modules/local/cocorv/main.nf#L257)

  ```nextflow
  publishDir "${params.outdir}/gnomADPosition", mode: 'copy'
  ```

- [`modules/local/cocorv/main.nf:278`](https://github.com/nf-core/rarevariantburden/blob/e9392c4294ecdd4f6f984b9c235eb220306455be/modules/local/cocorv/main.nf#L278)

  ```nextflow
  publishDir "${params.outdir}/gnomADPosition", mode: 'copy'
  ```

- [`modules/local/cocorv/main.nf:297`](https://github.com/nf-core/rarevariantburden/blob/e9392c4294ecdd4f6f984b9c235eb220306455be/modules/local/cocorv/main.nf#L297)

  ```nextflow
  publishDir "${params.outdir}/gnomADPosition", mode: 'copy'
  ```

- [`modules/local/cocorv/main.nf:325`](https://github.com/nf-core/rarevariantburden/blob/e9392c4294ecdd4f6f984b9c235eb220306455be/modules/local/cocorv/main.nf#L325)

  ```nextflow
  publishDir "${params.outdir}/gnomADPosition", mode: 'copy'
  ```

- [`modules/local/cocorv/main.nf:345`](https://github.com/nf-core/rarevariantburden/blob/e9392c4294ecdd4f6f984b9c235eb220306455be/modules/local/cocorv/main.nf#L345)

  ```nextflow
  publishDir "${params.outdir}/CoCoRV/byChr", mode: 'copy'
  ```

- [`modules/local/cocorv/main.nf:449`](https://github.com/nf-core/rarevariantburden/blob/e9392c4294ecdd4f6f984b9c235eb220306455be/modules/local/cocorv/main.nf#L449)

  ```nextflow
  publishDir "${params.outdir}/CoCoRV", mode: 'copy'
  ```

- [`modules/local/cocorv/main.nf:489`](https://github.com/nf-core/rarevariantburden/blob/e9392c4294ecdd4f6f984b9c235eb220306455be/modules/local/cocorv/main.nf#L489)

  ```nextflow
  publishDir "${params.outdir}/CoCoRV", mode: 'copy'
  ```

- [`modules/local/cocorv/main.nf:517`](https://github.com/nf-core/rarevariantburden/blob/e9392c4294ecdd4f6f984b9c235eb220306455be/modules/local/cocorv/main.nf#L517)

  ```nextflow
  publishDir "${params.outdir}/CoCoRV", mode: 'copy'
  ```

- [`modules/local/cocorv/main.nf:573`](https://github.com/nf-core/rarevariantburden/blob/e9392c4294ecdd4f6f984b9c235eb220306455be/modules/local/cocorv/main.nf#L573)

  ```nextflow
  publishDir "${params.outdir}/CoCoRV", mode: 'copy'
  ```
