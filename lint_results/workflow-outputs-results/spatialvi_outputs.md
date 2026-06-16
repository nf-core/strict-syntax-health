# Workflow outputs migration: spatialvi

- Generated: 2026-06-16T14:36:20.009105+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 13 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:17`](https://github.com/nf-core/spatialvi/blob/d0fd35d9a985b30db9895c8b4b08f291a700f722/conf/modules.config#L17)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:27`](https://github.com/nf-core/spatialvi/blob/d0fd35d9a985b30db9895c8b4b08f291a700f722/conf/modules.config#L27)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:37`](https://github.com/nf-core/spatialvi/blob/d0fd35d9a985b30db9895c8b4b08f291a700f722/conf/modules.config#L37)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:45`](https://github.com/nf-core/spatialvi/blob/d0fd35d9a985b30db9895c8b4b08f291a700f722/conf/modules.config#L45)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:53`](https://github.com/nf-core/spatialvi/blob/d0fd35d9a985b30db9895c8b4b08f291a700f722/conf/modules.config#L53)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:63`](https://github.com/nf-core/spatialvi/blob/d0fd35d9a985b30db9895c8b4b08f291a700f722/conf/modules.config#L63)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:77`](https://github.com/nf-core/spatialvi/blob/d0fd35d9a985b30db9895c8b4b08f291a700f722/conf/modules.config#L77)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:99`](https://github.com/nf-core/spatialvi/blob/d0fd35d9a985b30db9895c8b4b08f291a700f722/conf/modules.config#L99)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:108`](https://github.com/nf-core/spatialvi/blob/d0fd35d9a985b30db9895c8b4b08f291a700f722/conf/modules.config#L108)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:116`](https://github.com/nf-core/spatialvi/blob/d0fd35d9a985b30db9895c8b4b08f291a700f722/conf/modules.config#L116)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:126`](https://github.com/nf-core/spatialvi/blob/d0fd35d9a985b30db9895c8b4b08f291a700f722/conf/modules.config#L126)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:151`](https://github.com/nf-core/spatialvi/blob/d0fd35d9a985b30db9895c8b4b08f291a700f722/conf/modules.config#L151)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:107`](https://github.com/nf-core/spatialvi/blob/d0fd35d9a985b30db9895c8b4b08f291a700f722/nextflow.config#L107)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
