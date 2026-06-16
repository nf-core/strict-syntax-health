# Workflow outputs migration: lsmquant

- Generated: 2026-06-16T14:20:54.692603+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 10 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/lsmquant/blob/44374c995f674f9948cd9012f5efd5c28e90f20f/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/lsmquant/blob/44374c995f674f9948cd9012f5efd5c28e90f20f/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:31`](https://github.com/nf-core/lsmquant/blob/44374c995f674f9948cd9012f5efd5c28e90f20f/conf/modules.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:40`](https://github.com/nf-core/lsmquant/blob/44374c995f674f9948cd9012f5efd5c28e90f20f/conf/modules.config#L40)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:58`](https://github.com/nf-core/lsmquant/blob/44374c995f674f9948cd9012f5efd5c28e90f20f/conf/modules.config#L58)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:76`](https://github.com/nf-core/lsmquant/blob/44374c995f674f9948cd9012f5efd5c28e90f20f/conf/modules.config#L76)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:91`](https://github.com/nf-core/lsmquant/blob/44374c995f674f9948cd9012f5efd5c28e90f20f/conf/modules.config#L91)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:105`](https://github.com/nf-core/lsmquant/blob/44374c995f674f9948cd9012f5efd5c28e90f20f/conf/modules.config#L105)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:119`](https://github.com/nf-core/lsmquant/blob/44374c995f674f9948cd9012f5efd5c28e90f20f/conf/modules.config#L119)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:53`](https://github.com/nf-core/lsmquant/blob/44374c995f674f9948cd9012f5efd5c28e90f20f/nextflow.config#L53)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
