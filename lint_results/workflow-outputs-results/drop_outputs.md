# Workflow outputs migration: drop

- Generated: 2026-06-16T14:14:53.123929+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 34 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:35`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L35)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:48`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L48)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:61`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L61)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:70`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L70)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:89`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L89)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:102`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L102)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:115`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L115)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:172`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L172)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:181`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L181)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:199`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L199)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:211`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L211)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:223`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L223)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:235`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L235)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:247`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L247)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:264`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L264)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:277`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L277)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:290`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L290)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:303`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L303)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:317`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L317)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:330`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L330)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:342`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L342)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:354`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L354)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:377`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L377)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:400`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L400)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:423`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L423)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:446`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L446)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:469`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L469)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:493`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/conf/modules.config#L493)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/local/aberrantexpression/main.nf:269`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/subworkflows/local/aberrantexpression/main.nf#L269)

  ```nextflow
  def tag   = "${meta.id}__${meta.drop_group}" // tag for publishDir
  ```

- [`subworkflows/local/aberrantexpression/main.nf:322`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/subworkflows/local/aberrantexpression/main.nf#L322)

  ```nextflow
  def tag   = "${meta.id}__${meta.drop_group}" // tag for publishDir
  ```

- [`subworkflows/local/aberrantsplicing/main.nf:441`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/subworkflows/local/aberrantsplicing/main.nf#L441)

  ```nextflow
  def tag   = "${meta.id}" // tag for publishDir
  ```

- [`subworkflows/local/aberrantsplicing/main.nf:489`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/subworkflows/local/aberrantsplicing/main.nf#L489)

  ```nextflow
  def tag   = "${meta.id}" // tag for publishDir
  ```

- [`subworkflows/local/mae/main.nf:185`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/subworkflows/local/mae/main.nf#L185)

  ```nextflow
  def tag   = "${meta.id}" // tag for publishDir
  ```

- [`subworkflows/local/mae/main.nf:232`](https://github.com/nf-core/drop/blob/f1266ac313adb9eb5129eb761874eabe54629d87/subworkflows/local/mae/main.nf#L232)

  ```nextflow
  def tag   = "${meta.id}" // tag for publishDir
  ```
