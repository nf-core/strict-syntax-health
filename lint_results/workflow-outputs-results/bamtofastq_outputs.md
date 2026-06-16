# Workflow outputs migration: bamtofastq

- Generated: 2026-06-16T14:09:39.183838+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 18 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/bamtofastq/blob/665440cdcccfec66ceb8212589a3c6ee92920d49/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:33`](https://github.com/nf-core/bamtofastq/blob/665440cdcccfec66ceb8212589a3c6ee92920d49/conf/modules.config#L33)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:42`](https://github.com/nf-core/bamtofastq/blob/665440cdcccfec66ceb8212589a3c6ee92920d49/conf/modules.config#L42)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:53`](https://github.com/nf-core/bamtofastq/blob/665440cdcccfec66ceb8212589a3c6ee92920d49/conf/modules.config#L53)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:62`](https://github.com/nf-core/bamtofastq/blob/665440cdcccfec66ceb8212589a3c6ee92920d49/conf/modules.config#L62)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:70`](https://github.com/nf-core/bamtofastq/blob/665440cdcccfec66ceb8212589a3c6ee92920d49/conf/modules.config#L70)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:77`](https://github.com/nf-core/bamtofastq/blob/665440cdcccfec66ceb8212589a3c6ee92920d49/conf/modules.config#L77)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:86`](https://github.com/nf-core/bamtofastq/blob/665440cdcccfec66ceb8212589a3c6ee92920d49/conf/modules.config#L86)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:95`](https://github.com/nf-core/bamtofastq/blob/665440cdcccfec66ceb8212589a3c6ee92920d49/conf/modules.config#L95)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:103`](https://github.com/nf-core/bamtofastq/blob/665440cdcccfec66ceb8212589a3c6ee92920d49/conf/modules.config#L103)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:109`](https://github.com/nf-core/bamtofastq/blob/665440cdcccfec66ceb8212589a3c6ee92920d49/conf/modules.config#L109)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:117`](https://github.com/nf-core/bamtofastq/blob/665440cdcccfec66ceb8212589a3c6ee92920d49/conf/modules.config#L117)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:125`](https://github.com/nf-core/bamtofastq/blob/665440cdcccfec66ceb8212589a3c6ee92920d49/conf/modules.config#L125)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:133`](https://github.com/nf-core/bamtofastq/blob/665440cdcccfec66ceb8212589a3c6ee92920d49/conf/modules.config#L133)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:140`](https://github.com/nf-core/bamtofastq/blob/665440cdcccfec66ceb8212589a3c6ee92920d49/conf/modules.config#L140)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:146`](https://github.com/nf-core/bamtofastq/blob/665440cdcccfec66ceb8212589a3c6ee92920d49/conf/modules.config#L146)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:156`](https://github.com/nf-core/bamtofastq/blob/665440cdcccfec66ceb8212589a3c6ee92920d49/conf/modules.config#L156)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:61`](https://github.com/nf-core/bamtofastq/blob/665440cdcccfec66ceb8212589a3c6ee92920d49/nextflow.config#L61)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
