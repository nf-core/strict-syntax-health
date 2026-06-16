# Workflow outputs migration: spatialaxe

- Generated: 2026-06-16T14:36:02.552082+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 39 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:25`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L25)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:34`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L34)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:43`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L43)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:60`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L60)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:67`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L67)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:81`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L81)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:93`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L93)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:103`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L103)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:116`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L116)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:124`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L124)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:131`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L131)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:138`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L138)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:146`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L146)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:158`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L158)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:170`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L170)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:180`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L180)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:192`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L192)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:205`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L205)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:221`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L221)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:232`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L232)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:239`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L239)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:246`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L246)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:253`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L253)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:260`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L260)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:267`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L267)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:274`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L274)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:281`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L281)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:290`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L290)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:298`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L298)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:305`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L305)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:315`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L315)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:323`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L323)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:341`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L341)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:349`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L349)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:356`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L356)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:365`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L365)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:372`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L372)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:379`](https://github.com/nf-core/spatialaxe/blob/d1eaf0f06da8f36525bacdd8b4bbedb110585c9e/conf/modules.config#L379)

  ```nextflow
  publishDir = [
  ```
