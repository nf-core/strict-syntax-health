# Workflow outputs migration: tumourevo

- Generated: 2026-06-16T14:37:50.099481+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 21 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:4`](https://github.com/nf-core/tumourevo/blob/43cc20b77aa9e74754cf4b15766081216a1d508e/conf/modules.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:14`](https://github.com/nf-core/tumourevo/blob/43cc20b77aa9e74754cf4b15766081216a1d508e/conf/modules.config#L14)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:47`](https://github.com/nf-core/tumourevo/blob/43cc20b77aa9e74754cf4b15766081216a1d508e/conf/modules.config#L47)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:63`](https://github.com/nf-core/tumourevo/blob/43cc20b77aa9e74754cf4b15766081216a1d508e/conf/modules.config#L63)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:73`](https://github.com/nf-core/tumourevo/blob/43cc20b77aa9e74754cf4b15766081216a1d508e/conf/modules.config#L73)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:85`](https://github.com/nf-core/tumourevo/blob/43cc20b77aa9e74754cf4b15766081216a1d508e/conf/modules.config#L85)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:97`](https://github.com/nf-core/tumourevo/blob/43cc20b77aa9e74754cf4b15766081216a1d508e/conf/modules.config#L97)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:107`](https://github.com/nf-core/tumourevo/blob/43cc20b77aa9e74754cf4b15766081216a1d508e/conf/modules.config#L107)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:117`](https://github.com/nf-core/tumourevo/blob/43cc20b77aa9e74754cf4b15766081216a1d508e/conf/modules.config#L117)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:127`](https://github.com/nf-core/tumourevo/blob/43cc20b77aa9e74754cf4b15766081216a1d508e/conf/modules.config#L127)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:136`](https://github.com/nf-core/tumourevo/blob/43cc20b77aa9e74754cf4b15766081216a1d508e/conf/modules.config#L136)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:146`](https://github.com/nf-core/tumourevo/blob/43cc20b77aa9e74754cf4b15766081216a1d508e/conf/modules.config#L146)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:156`](https://github.com/nf-core/tumourevo/blob/43cc20b77aa9e74754cf4b15766081216a1d508e/conf/modules.config#L156)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:166`](https://github.com/nf-core/tumourevo/blob/43cc20b77aa9e74754cf4b15766081216a1d508e/conf/modules.config#L166)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:178`](https://github.com/nf-core/tumourevo/blob/43cc20b77aa9e74754cf4b15766081216a1d508e/conf/modules.config#L178)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:188`](https://github.com/nf-core/tumourevo/blob/43cc20b77aa9e74754cf4b15766081216a1d508e/conf/modules.config#L188)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:207`](https://github.com/nf-core/tumourevo/blob/43cc20b77aa9e74754cf4b15766081216a1d508e/conf/modules.config#L207)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:239`](https://github.com/nf-core/tumourevo/blob/43cc20b77aa9e74754cf4b15766081216a1d508e/conf/modules.config#L239)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:263`](https://github.com/nf-core/tumourevo/blob/43cc20b77aa9e74754cf4b15766081216a1d508e/conf/modules.config#L263)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:277`](https://github.com/nf-core/tumourevo/blob/43cc20b77aa9e74754cf4b15766081216a1d508e/conf/modules.config#L277)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:287`](https://github.com/nf-core/tumourevo/blob/43cc20b77aa9e74754cf4b15766081216a1d508e/conf/modules.config#L287)

  ```nextflow
  publishDir = [
  ```
