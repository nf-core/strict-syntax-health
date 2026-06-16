# Workflow outputs migration: metapep

- Generated: 2026-06-16T14:22:16.917445+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 21 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/metapep/blob/034ac0e8afd267c78cabef85b96dc6c8d3952098/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:22`](https://github.com/nf-core/metapep/blob/034ac0e8afd267c78cabef85b96dc6c8d3952098/conf/modules.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:30`](https://github.com/nf-core/metapep/blob/034ac0e8afd267c78cabef85b96dc6c8d3952098/conf/modules.config#L30)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:39`](https://github.com/nf-core/metapep/blob/034ac0e8afd267c78cabef85b96dc6c8d3952098/conf/modules.config#L39)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:45`](https://github.com/nf-core/metapep/blob/034ac0e8afd267c78cabef85b96dc6c8d3952098/conf/modules.config#L45)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:53`](https://github.com/nf-core/metapep/blob/034ac0e8afd267c78cabef85b96dc6c8d3952098/conf/modules.config#L53)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:64`](https://github.com/nf-core/metapep/blob/034ac0e8afd267c78cabef85b96dc6c8d3952098/conf/modules.config#L64)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:72`](https://github.com/nf-core/metapep/blob/034ac0e8afd267c78cabef85b96dc6c8d3952098/conf/modules.config#L72)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:79`](https://github.com/nf-core/metapep/blob/034ac0e8afd267c78cabef85b96dc6c8d3952098/conf/modules.config#L79)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:84`](https://github.com/nf-core/metapep/blob/034ac0e8afd267c78cabef85b96dc6c8d3952098/conf/modules.config#L84)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:89`](https://github.com/nf-core/metapep/blob/034ac0e8afd267c78cabef85b96dc6c8d3952098/conf/modules.config#L89)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:95`](https://github.com/nf-core/metapep/blob/034ac0e8afd267c78cabef85b96dc6c8d3952098/conf/modules.config#L95)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:101`](https://github.com/nf-core/metapep/blob/034ac0e8afd267c78cabef85b96dc6c8d3952098/conf/modules.config#L101)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:106`](https://github.com/nf-core/metapep/blob/034ac0e8afd267c78cabef85b96dc6c8d3952098/conf/modules.config#L106)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:110`](https://github.com/nf-core/metapep/blob/034ac0e8afd267c78cabef85b96dc6c8d3952098/conf/modules.config#L110)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:116`](https://github.com/nf-core/metapep/blob/034ac0e8afd267c78cabef85b96dc6c8d3952098/conf/modules.config#L116)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:124`](https://github.com/nf-core/metapep/blob/034ac0e8afd267c78cabef85b96dc6c8d3952098/conf/modules.config#L124)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:132`](https://github.com/nf-core/metapep/blob/034ac0e8afd267c78cabef85b96dc6c8d3952098/conf/modules.config#L132)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:140`](https://github.com/nf-core/metapep/blob/034ac0e8afd267c78cabef85b96dc6c8d3952098/conf/modules.config#L140)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:148`](https://github.com/nf-core/metapep/blob/034ac0e8afd267c78cabef85b96dc6c8d3952098/conf/modules.config#L148)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:156`](https://github.com/nf-core/metapep/blob/034ac0e8afd267c78cabef85b96dc6c8d3952098/conf/modules.config#L156)

  ```nextflow
  publishDir = [
  ```
