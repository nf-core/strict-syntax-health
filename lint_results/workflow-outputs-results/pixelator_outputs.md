# Workflow outputs migration: pixelator

- Generated: 2026-06-16T14:27:32.366700+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 13 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:16`](https://github.com/nf-core/pixelator/blob/5050af76b11148e4fe5366e6ba831805bcf9965f/conf/modules.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/pixelator/blob/5050af76b11148e4fe5366e6ba831805bcf9965f/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:38`](https://github.com/nf-core/pixelator/blob/5050af76b11148e4fe5366e6ba831805bcf9965f/conf/modules.config#L38)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:42`](https://github.com/nf-core/pixelator/blob/5050af76b11148e4fe5366e6ba831805bcf9965f/conf/modules.config#L42)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.pna.config:30`](https://github.com/nf-core/pixelator/blob/5050af76b11148e4fe5366e6ba831805bcf9965f/conf/modules.pna.config#L30)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.pna.config:60`](https://github.com/nf-core/pixelator/blob/5050af76b11148e4fe5366e6ba831805bcf9965f/conf/modules.pna.config#L60)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.pna.config:100`](https://github.com/nf-core/pixelator/blob/5050af76b11148e4fe5366e6ba831805bcf9965f/conf/modules.pna.config#L100)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.pna.config:137`](https://github.com/nf-core/pixelator/blob/5050af76b11148e4fe5366e6ba831805bcf9965f/conf/modules.pna.config#L137)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.pna.config:166`](https://github.com/nf-core/pixelator/blob/5050af76b11148e4fe5366e6ba831805bcf9965f/conf/modules.pna.config#L166)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.pna.config:200`](https://github.com/nf-core/pixelator/blob/5050af76b11148e4fe5366e6ba831805bcf9965f/conf/modules.pna.config#L200)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.pna.config:234`](https://github.com/nf-core/pixelator/blob/5050af76b11148e4fe5366e6ba831805bcf9965f/conf/modules.pna.config#L234)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.pna.config:265`](https://github.com/nf-core/pixelator/blob/5050af76b11148e4fe5366e6ba831805bcf9965f/conf/modules.pna.config#L265)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:139`](https://github.com/nf-core/pixelator/blob/5050af76b11148e4fe5366e6ba831805bcf9965f/nextflow.config#L139)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
