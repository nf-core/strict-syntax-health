# Workflow outputs migration: variantcatalogue

- Generated: 2026-06-16T14:38:27.824265+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 33 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:22`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:36`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L36)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:47`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L47)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:54`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L54)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:60`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L60)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:70`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L70)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:80`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L80)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:96`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L96)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:107`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L107)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:115`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L115)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:121`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L121)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:128`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L128)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:139`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L139)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:154`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L154)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:179`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L179)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:200`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L200)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:206`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L206)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:214`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L214)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:222`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L222)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:228`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L228)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:236`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L236)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:247`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L247)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:254`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L254)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:264`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L264)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:270`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L270)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:277`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L277)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:284`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L284)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:294`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L294)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:300`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L300)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:310`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L310)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:317`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L317)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:351`](https://github.com/nf-core/variantcatalogue/blob/46154522d37b22694edce7b2e75af11e1c28ca26/conf/modules.config#L351)

  ```nextflow
  publishDir = [
  ```
