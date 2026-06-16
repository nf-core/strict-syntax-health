# Workflow outputs migration: pairgenomealign

- Generated: 2026-06-16T14:26:02.994452+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 12 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/pairgenomealign/blob/f6756c6e3e1079c9f5f5bcce14ccbf33f0a21396/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:39`](https://github.com/nf-core/pairgenomealign/blob/f6756c6e3e1079c9f5f5bcce14ccbf33f0a21396/conf/modules.config#L39)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:69`](https://github.com/nf-core/pairgenomealign/blob/f6756c6e3e1079c9f5f5bcce14ccbf33f0a21396/conf/modules.config#L69)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:115`](https://github.com/nf-core/pairgenomealign/blob/f6756c6e3e1079c9f5f5bcce14ccbf33f0a21396/conf/modules.config#L115)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:126`](https://github.com/nf-core/pairgenomealign/blob/f6756c6e3e1079c9f5f5bcce14ccbf33f0a21396/conf/modules.config#L126)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:133`](https://github.com/nf-core/pairgenomealign/blob/f6756c6e3e1079c9f5f5bcce14ccbf33f0a21396/conf/modules.config#L133)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:143`](https://github.com/nf-core/pairgenomealign/blob/f6756c6e3e1079c9f5f5bcce14ccbf33f0a21396/conf/modules.config#L143)

  ```nextflow
  publishDir    = [ enabled: false ]
  ```

- [`conf/modules.config:147`](https://github.com/nf-core/pairgenomealign/blob/f6756c6e3e1079c9f5f5bcce14ccbf33f0a21396/conf/modules.config#L147)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:156`](https://github.com/nf-core/pairgenomealign/blob/f6756c6e3e1079c9f5f5bcce14ccbf33f0a21396/conf/modules.config#L156)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:163`](https://github.com/nf-core/pairgenomealign/blob/f6756c6e3e1079c9f5f5bcce14ccbf33f0a21396/conf/modules.config#L163)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:172`](https://github.com/nf-core/pairgenomealign/blob/f6756c6e3e1079c9f5f5bcce14ccbf33f0a21396/conf/modules.config#L172)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:89`](https://github.com/nf-core/pairgenomealign/blob/f6756c6e3e1079c9f5f5bcce14ccbf33f0a21396/nextflow.config#L89)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
