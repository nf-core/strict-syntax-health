# Workflow outputs migration: epitopeprediction

- Generated: 2026-06-16T14:16:02.687757+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 19 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/epitopeprediction/blob/4da770321a335c8aff6cb713a78dd1e755ad116c/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:22`](https://github.com/nf-core/epitopeprediction/blob/4da770321a335c8aff6cb713a78dd1e755ad116c/conf/modules.config#L22)

  ```nextflow
  publishDir  = [ enabled: false ]
  ```

- [`conf/modules.config:26`](https://github.com/nf-core/epitopeprediction/blob/4da770321a335c8aff6cb713a78dd1e755ad116c/conf/modules.config#L26)

  ```nextflow
  publishDir  = [ enabled: false ]
  ```

- [`conf/modules.config:32`](https://github.com/nf-core/epitopeprediction/blob/4da770321a335c8aff6cb713a78dd1e755ad116c/conf/modules.config#L32)

  ```nextflow
  publishDir  = [ enabled: false ]
  ```

- [`conf/modules.config:36`](https://github.com/nf-core/epitopeprediction/blob/4da770321a335c8aff6cb713a78dd1e755ad116c/conf/modules.config#L36)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:43`](https://github.com/nf-core/epitopeprediction/blob/4da770321a335c8aff6cb713a78dd1e755ad116c/conf/modules.config#L43)

  ```nextflow
  publishDir  = [ enabled: false ]
  ```

- [`conf/modules.config:55`](https://github.com/nf-core/epitopeprediction/blob/4da770321a335c8aff6cb713a78dd1e755ad116c/conf/modules.config#L55)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:63`](https://github.com/nf-core/epitopeprediction/blob/4da770321a335c8aff6cb713a78dd1e755ad116c/conf/modules.config#L63)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:71`](https://github.com/nf-core/epitopeprediction/blob/4da770321a335c8aff6cb713a78dd1e755ad116c/conf/modules.config#L71)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:75`](https://github.com/nf-core/epitopeprediction/blob/4da770321a335c8aff6cb713a78dd1e755ad116c/conf/modules.config#L75)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:81`](https://github.com/nf-core/epitopeprediction/blob/4da770321a335c8aff6cb713a78dd1e755ad116c/conf/modules.config#L81)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:86`](https://github.com/nf-core/epitopeprediction/blob/4da770321a335c8aff6cb713a78dd1e755ad116c/conf/modules.config#L86)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:95`](https://github.com/nf-core/epitopeprediction/blob/4da770321a335c8aff6cb713a78dd1e755ad116c/conf/modules.config#L95)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:105`](https://github.com/nf-core/epitopeprediction/blob/4da770321a335c8aff6cb713a78dd1e755ad116c/conf/modules.config#L105)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:115`](https://github.com/nf-core/epitopeprediction/blob/4da770321a335c8aff6cb713a78dd1e755ad116c/conf/modules.config#L115)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:128`](https://github.com/nf-core/epitopeprediction/blob/4da770321a335c8aff6cb713a78dd1e755ad116c/conf/modules.config#L128)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:136`](https://github.com/nf-core/epitopeprediction/blob/4da770321a335c8aff6cb713a78dd1e755ad116c/conf/modules.config#L136)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:145`](https://github.com/nf-core/epitopeprediction/blob/4da770321a335c8aff6cb713a78dd1e755ad116c/conf/modules.config#L145)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:87`](https://github.com/nf-core/epitopeprediction/blob/4da770321a335c8aff6cb713a78dd1e755ad116c/nextflow.config#L87)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
