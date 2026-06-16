# Workflow outputs migration: variantprioritization

- Generated: 2026-06-16T14:38:34.322404+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 14 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/variantprioritization/blob/b3e275d2ec72773be2245ed14d871264deae057d/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/variantprioritization/blob/b3e275d2ec72773be2245ed14d871264deae057d/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:40`](https://github.com/nf-core/variantprioritization/blob/b3e275d2ec72773be2245ed14d871264deae057d/conf/modules.config#L40)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:66`](https://github.com/nf-core/variantprioritization/blob/b3e275d2ec72773be2245ed14d871264deae057d/conf/modules.config#L66)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:74`](https://github.com/nf-core/variantprioritization/blob/b3e275d2ec72773be2245ed14d871264deae057d/conf/modules.config#L74)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:82`](https://github.com/nf-core/variantprioritization/blob/b3e275d2ec72773be2245ed14d871264deae057d/conf/modules.config#L82)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:90`](https://github.com/nf-core/variantprioritization/blob/b3e275d2ec72773be2245ed14d871264deae057d/conf/modules.config#L90)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:100`](https://github.com/nf-core/variantprioritization/blob/b3e275d2ec72773be2245ed14d871264deae057d/conf/modules.config#L100)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:109`](https://github.com/nf-core/variantprioritization/blob/b3e275d2ec72773be2245ed14d871264deae057d/conf/modules.config#L109)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:117`](https://github.com/nf-core/variantprioritization/blob/b3e275d2ec72773be2245ed14d871264deae057d/conf/modules.config#L117)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:126`](https://github.com/nf-core/variantprioritization/blob/b3e275d2ec72773be2245ed14d871264deae057d/conf/modules.config#L126)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:192`](https://github.com/nf-core/variantprioritization/blob/b3e275d2ec72773be2245ed14d871264deae057d/conf/modules.config#L192)

  ```nextflow
  publishDir   = [
  ```

- [`conf/modules.config:222`](https://github.com/nf-core/variantprioritization/blob/b3e275d2ec72773be2245ed14d871264deae057d/conf/modules.config#L222)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:149`](https://github.com/nf-core/variantprioritization/blob/b3e275d2ec72773be2245ed14d871264deae057d/nextflow.config#L149)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
