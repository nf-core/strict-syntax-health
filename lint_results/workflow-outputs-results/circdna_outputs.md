# Workflow outputs migration: circdna

- Generated: 2026-06-16T14:10:44.979111+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 36 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:16`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:24`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L24)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:37`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L37)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:51`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L51)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:61`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L61)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:77`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L77)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:97`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L97)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:127`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L127)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:137`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L137)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:148`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L148)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:161`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L161)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:182`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L182)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:201`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L201)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:211`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L211)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:220`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L220)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:232`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L232)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:244`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L244)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:261`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L261)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:270`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L270)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:280`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L280)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:290`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L290)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:299`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L299)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:314`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L314)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:330`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L330)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:402`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L402)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:412`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L412)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:423`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L423)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:434`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L434)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:444`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L444)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:454`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L454)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:470`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L470)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:480`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L480)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:490`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L490)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:501`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L501)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:515`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L515)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:523`](https://github.com/nf-core/circdna/blob/b5e2fbe05c2892f963e7e02784efd657d429634d/conf/modules.config#L523)

  ```nextflow
  publishDir = [
  ```
