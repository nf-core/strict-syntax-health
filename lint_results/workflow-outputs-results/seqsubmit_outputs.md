# Workflow outputs migration: seqsubmit

- Generated: 2026-06-16T14:35:15.959324+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 21 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/seqsubmit/blob/b8cbf9b6fdf3f1a1be78ae47b9aef80870d65963/conf/modules.config#L15)

  ```nextflow
  // Default publishDir for all processes, can be overridden by individual process definitions below
  ```

- [`conf/modules.config:16`](https://github.com/nf-core/seqsubmit/blob/b8cbf9b6fdf3f1a1be78ae47b9aef80870d65963/conf/modules.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:27`](https://github.com/nf-core/seqsubmit/blob/b8cbf9b6fdf3f1a1be78ae47b9aef80870d65963/conf/modules.config#L27)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:38`](https://github.com/nf-core/seqsubmit/blob/b8cbf9b6fdf3f1a1be78ae47b9aef80870d65963/conf/modules.config#L38)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:46`](https://github.com/nf-core/seqsubmit/blob/b8cbf9b6fdf3f1a1be78ae47b9aef80870d65963/conf/modules.config#L46)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:54`](https://github.com/nf-core/seqsubmit/blob/b8cbf9b6fdf3f1a1be78ae47b9aef80870d65963/conf/modules.config#L54)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:71`](https://github.com/nf-core/seqsubmit/blob/b8cbf9b6fdf3f1a1be78ae47b9aef80870d65963/conf/modules.config#L71)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:81`](https://github.com/nf-core/seqsubmit/blob/b8cbf9b6fdf3f1a1be78ae47b9aef80870d65963/conf/modules.config#L81)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:89`](https://github.com/nf-core/seqsubmit/blob/b8cbf9b6fdf3f1a1be78ae47b9aef80870d65963/conf/modules.config#L89)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:97`](https://github.com/nf-core/seqsubmit/blob/b8cbf9b6fdf3f1a1be78ae47b9aef80870d65963/conf/modules.config#L97)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:107`](https://github.com/nf-core/seqsubmit/blob/b8cbf9b6fdf3f1a1be78ae47b9aef80870d65963/conf/modules.config#L107)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:115`](https://github.com/nf-core/seqsubmit/blob/b8cbf9b6fdf3f1a1be78ae47b9aef80870d65963/conf/modules.config#L115)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:128`](https://github.com/nf-core/seqsubmit/blob/b8cbf9b6fdf3f1a1be78ae47b9aef80870d65963/conf/modules.config#L128)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:136`](https://github.com/nf-core/seqsubmit/blob/b8cbf9b6fdf3f1a1be78ae47b9aef80870d65963/conf/modules.config#L136)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:148`](https://github.com/nf-core/seqsubmit/blob/b8cbf9b6fdf3f1a1be78ae47b9aef80870d65963/conf/modules.config#L148)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:154`](https://github.com/nf-core/seqsubmit/blob/b8cbf9b6fdf3f1a1be78ae47b9aef80870d65963/conf/modules.config#L154)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:163`](https://github.com/nf-core/seqsubmit/blob/b8cbf9b6fdf3f1a1be78ae47b9aef80870d65963/conf/modules.config#L163)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:172`](https://github.com/nf-core/seqsubmit/blob/b8cbf9b6fdf3f1a1be78ae47b9aef80870d65963/conf/modules.config#L172)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:180`](https://github.com/nf-core/seqsubmit/blob/b8cbf9b6fdf3f1a1be78ae47b9aef80870d65963/conf/modules.config#L180)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:196`](https://github.com/nf-core/seqsubmit/blob/b8cbf9b6fdf3f1a1be78ae47b9aef80870d65963/conf/modules.config#L196)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:68`](https://github.com/nf-core/seqsubmit/blob/b8cbf9b6fdf3f1a1be78ae47b9aef80870d65963/nextflow.config#L68)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
