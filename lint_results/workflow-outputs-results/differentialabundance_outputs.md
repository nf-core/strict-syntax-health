# Workflow outputs migration: differentialabundance

- Generated: 2026-06-16T14:14:15.562214+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:275`](https://github.com/nf-core/differentialabundance/blob/16da8b78a33418e18145b19156e3b7663b7a9037/main.nf#L275)

  ```nextflow
  output {
  ```

## Legacy `publishDir` references

Found 10 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:255`](https://github.com/nf-core/differentialabundance/blob/16da8b78a33418e18145b19156e3b7663b7a9037/conf/modules.config#L255)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:383`](https://github.com/nf-core/differentialabundance/blob/16da8b78a33418e18145b19156e3b7663b7a9037/conf/modules.config#L383)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/limma/differential/tests/nextflow.config:12`](https://github.com/nf-core/differentialabundance/blob/16da8b78a33418e18145b19156e3b7663b7a9037/modules/nf-core/limma/differential/tests/nextflow.config#L12)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`modules/nf-core/limma/differential/tests/nextflow.config:15`](https://github.com/nf-core/differentialabundance/blob/16da8b78a33418e18145b19156e3b7663b7a9037/modules/nf-core/limma/differential/tests/nextflow.config#L15)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`modules/nf-core/limma/differential/tests/nextflow.exclude_samples.config:13`](https://github.com/nf-core/differentialabundance/blob/16da8b78a33418e18145b19156e3b7663b7a9037/modules/nf-core/limma/differential/tests/nextflow.exclude_samples.config#L13)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`modules/nf-core/limma/differential/tests/nextflow.exclude_samples.config:17`](https://github.com/nf-core/differentialabundance/blob/16da8b78a33418e18145b19156e3b7663b7a9037/modules/nf-core/limma/differential/tests/nextflow.exclude_samples.config#L17)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`modules/nf-core/limma/differential/tests/nextflow.subset_to_contrast.config:12`](https://github.com/nf-core/differentialabundance/blob/16da8b78a33418e18145b19156e3b7663b7a9037/modules/nf-core/limma/differential/tests/nextflow.subset_to_contrast.config#L12)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`modules/nf-core/limma/differential/tests/nextflow.subset_to_contrast.config:16`](https://github.com/nf-core/differentialabundance/blob/16da8b78a33418e18145b19156e3b7663b7a9037/modules/nf-core/limma/differential/tests/nextflow.subset_to_contrast.config#L16)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`subworkflows/nf-core/abundance_differential_filter/tests/limma_basic_microarray.config:18`](https://github.com/nf-core/differentialabundance/blob/16da8b78a33418e18145b19156e3b7663b7a9037/subworkflows/nf-core/abundance_differential_filter/tests/limma_basic_microarray.config#L18)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`subworkflows/nf-core/abundance_differential_filter/tests/limma_basic_microarray.config:21`](https://github.com/nf-core/differentialabundance/blob/16da8b78a33418e18145b19156e3b7663b7a9037/subworkflows/nf-core/abundance_differential_filter/tests/limma_basic_microarray.config#L21)

  ```nextflow
  publishDir = [ enabled: false ]
  ```
