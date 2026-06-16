# Workflow outputs migration: bacmodel

- Generated: 2026-06-16T14:09:17.008476+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 13 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/bacmodel/blob/30020a4d2a7a34782a324ce3c1357e8e824eb320/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/bacmodel/blob/30020a4d2a7a34782a324ce3c1357e8e824eb320/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:32`](https://github.com/nf-core/bacmodel/blob/30020a4d2a7a34782a324ce3c1357e8e824eb320/conf/modules.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:41`](https://github.com/nf-core/bacmodel/blob/30020a4d2a7a34782a324ce3c1357e8e824eb320/conf/modules.config#L41)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:50`](https://github.com/nf-core/bacmodel/blob/30020a4d2a7a34782a324ce3c1357e8e824eb320/conf/modules.config#L50)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:58`](https://github.com/nf-core/bacmodel/blob/30020a4d2a7a34782a324ce3c1357e8e824eb320/conf/modules.config#L58)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:67`](https://github.com/nf-core/bacmodel/blob/30020a4d2a7a34782a324ce3c1357e8e824eb320/conf/modules.config#L67)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:75`](https://github.com/nf-core/bacmodel/blob/30020a4d2a7a34782a324ce3c1357e8e824eb320/conf/modules.config#L75)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:84`](https://github.com/nf-core/bacmodel/blob/30020a4d2a7a34782a324ce3c1357e8e824eb320/conf/modules.config#L84)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:101`](https://github.com/nf-core/bacmodel/blob/30020a4d2a7a34782a324ce3c1357e8e824eb320/conf/modules.config#L101)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:110`](https://github.com/nf-core/bacmodel/blob/30020a4d2a7a34782a324ce3c1357e8e824eb320/conf/modules.config#L110)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:119`](https://github.com/nf-core/bacmodel/blob/30020a4d2a7a34782a324ce3c1357e8e824eb320/conf/modules.config#L119)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:128`](https://github.com/nf-core/bacmodel/blob/30020a4d2a7a34782a324ce3c1357e8e824eb320/conf/modules.config#L128)

  ```nextflow
  publishDir = [
  ```
