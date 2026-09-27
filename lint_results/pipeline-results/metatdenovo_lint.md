# Nextflow lint results

- Generated: 2026-09-27T00:22:38.730886612Z
- Nextflow version: 26.09.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `workflows/metatdenovo.nf:187:61`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def duplicate_user_orf_names = user_orf_names.countBy { it }.findAll { _name, count -> count > 1 }.keySet()
                                                              ^^
  ```
