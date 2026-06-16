# Workflow outputs migration: phaseimpute

- Generated: 2026-06-16T14:26:57.115321+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 85 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:22`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/modules.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:34`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/modules.config#L34)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:39`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/modules.config#L39)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:46`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/modules.config#L46)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:56`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/modules.config#L56)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:66`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/modules.config#L66)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/chrcheck.config:16`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/chrcheck.config#L16)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/steps/chrcheck.config:22`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/chrcheck.config#L22)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/steps/chrcheck.config:28`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/chrcheck.config#L28)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/steps/imputation_beagle5.config:18`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_beagle5.config#L18)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/steps/imputation_beagle5.config:26`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_beagle5.config#L26)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/steps/imputation_beagle5.config:33`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_beagle5.config#L33)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/steps/imputation_beagle5.config:39`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_beagle5.config#L39)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/steps/imputation_beagle5.config:46`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_beagle5.config#L46)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/steps/imputation_beagle5.config:51`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_beagle5.config#L51)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/steps/imputation_beagle5.config:56`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_beagle5.config#L56)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/imputation_glimpse1.config:18`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_glimpse1.config#L18)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/imputation_glimpse1.config:55`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_glimpse1.config#L55)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/imputation_glimpse1.config:84`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_glimpse1.config#L84)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/imputation_glimpse2.config:16`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_glimpse2.config#L16)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/steps/imputation_glimpse2.config:25`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_glimpse2.config#L25)

  ```nextflow
  publishDir   = [ enabled: false ]
  ```

- [`conf/steps/imputation_glimpse2.config:30`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_glimpse2.config#L30)

  ```nextflow
  publishDir   = [ enabled: false ]
  ```

- [`conf/steps/imputation_glimpse2.config:36`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_glimpse2.config#L36)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/steps/imputation_glimpse2.config:41`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_glimpse2.config#L41)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/steps/imputation_glimpse2.config:47`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_glimpse2.config#L47)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/imputation_minimac4.config:15`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_minimac4.config#L15)

  ```nextflow
  publishDir = [enabled: false]
  ```

- [`conf/steps/imputation_minimac4.config:45`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_minimac4.config#L45)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/imputation_quilt.config:16`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_quilt.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/imputation_quilt.config:40`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_quilt.config#L40)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/imputation_quilt2.config:10`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_quilt2.config#L10)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/imputation_quilt2.config:32`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_quilt2.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/imputation_shared.config:19`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_shared.config#L19)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/imputation_shared.config:31`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_shared.config#L31)

  ```nextflow
  publishDir = [enabled: false]
  ```

- [`conf/steps/imputation_shared.config:37`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_shared.config#L37)

  ```nextflow
  publishDir = [enabled: false]
  ```

- [`conf/steps/imputation_shared.config:45`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_shared.config#L45)

  ```nextflow
  publishDir = [enabled: false]
  ```

- [`conf/steps/imputation_shared.config:52`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_shared.config#L52)

  ```nextflow
  publishDir = [enabled: false]
  ```

- [`conf/steps/imputation_shared.config:59`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_shared.config#L59)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/imputation_stitch.config:16`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_stitch.config#L16)

  ```nextflow
  publishDir = [enabled: false]
  ```

- [`conf/steps/imputation_stitch.config:38`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/imputation_stitch.config#L38)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/initialisation.config:15`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/initialisation.config#L15)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/steps/initialisation.config:19`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/initialisation.config#L19)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/initialisation.config:30`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/initialisation.config#L30)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/panelprep.config:16`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/panelprep.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/panelprep.config:35`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/panelprep.config#L35)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/panelprep.config:50`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/panelprep.config#L50)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/panelprep.config:65`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/panelprep.config#L65)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/panelprep.config:80`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/panelprep.config#L80)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/panelprep.config:102`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/panelprep.config#L102)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/panelprep.config:112`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/panelprep.config#L112)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/panelprep.config:121`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/panelprep.config#L121)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/panelprep.config:131`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/panelprep.config#L131)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/panelprep.config:148`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/panelprep.config#L148)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/panelprep.config:163`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/panelprep.config#L163)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/panelprep.config:172`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/panelprep.config#L172)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/panelprep.config:193`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/panelprep.config#L193)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/panelprep.config:203`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/panelprep.config#L203)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/simulation.config:16`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/simulation.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/simulation.config:42`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/simulation.config#L42)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/simulation.config:65`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/simulation.config#L65)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/simulation.config:75`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/simulation.config#L75)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/steps/simulation.config:80`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/simulation.config#L80)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/steps/validation.config:18`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/validation.config#L18)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/steps/validation.config:47`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/validation.config#L47)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/validation.config:57`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/validation.config#L57)

  ```nextflow
  publishDir = [enabled: false]
  ```

- [`conf/steps/validation.config:64`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/validation.config#L64)

  ```nextflow
  publishDir = [enabled: false]
  ```

- [`conf/steps/validation.config:70`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/validation.config#L70)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/validation.config:78`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/validation.config#L78)

  ```nextflow
  publishDir = [
  ```

- [`conf/steps/validation.config:88`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/validation.config#L88)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/steps/validation.config:96`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/validation.config#L96)

  ```nextflow
  publishDir = [enabled: false]
  ```

- [`conf/steps/validation.config:104`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/validation.config#L104)

  ```nextflow
  publishDir = [enabled: false]
  ```

- [`conf/steps/validation.config:109`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/steps/validation.config#L109)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/test_all.config:53`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/test_all.config#L53)

  ```nextflow
  publishDir = [
  ```

- [`conf/test_all.config:63`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/test_all.config#L63)

  ```nextflow
  publishDir = [
  ```

- [`conf/test_dog.config:51`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/test_dog.config#L51)

  ```nextflow
  publishDir = [
  ```

- [`conf/test_dog.config:61`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/test_dog.config#L61)

  ```nextflow
  publishDir = [
  ```

- [`conf/test_full.config:46`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/test_full.config#L46)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/test_panelprep.config:48`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/test_panelprep.config#L48)

  ```nextflow
  publishDir = [
  ```

- [`conf/test_panelprep.config:58`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/conf/test_panelprep.config#L58)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:105`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/nextflow.config#L105)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```

- [`subworkflows/nf-core/bam_impute_quilt/tests/nextflow.config:14`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/subworkflows/nf-core/bam_impute_quilt/tests/nextflow.config#L14)

  ```nextflow
  publishDir = [enabled: false]
  ```

- [`tests/nextflow.config:19`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/tests/nextflow.config#L19)

  ```nextflow
  publishDir   = [ enabled: false ]
  ```

- [`workflows/phaseimpute/tests/nextflow.config:32`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/workflows/phaseimpute/tests/nextflow.config#L32)

  ```nextflow
  publishDir   = [ enabled: false ]
  ```

- [`workflows/phaseimpute/tests/nextflow.config:40`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/workflows/phaseimpute/tests/nextflow.config#L40)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`workflows/phaseimpute/tests/nextflow.config:46`](https://github.com/nf-core/phaseimpute/blob/52ee9d66325777d1f1cc684dd7347b63c2029144/workflows/phaseimpute/tests/nextflow.config#L46)

  ```nextflow
  publishDir = [ enabled: false ]
  ```
