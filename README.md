# p6m7g8-actions/p6-build

- [p6m7g8-actions/p6-build](#p6m7g8-actionsp6-build)
  - [Usage](#usage)

## Usage

```yaml
      - name: P6- build
        uses: p6m7g8-actions/p6-build@main
```

The composite checks out the workspace itself, as its first step, so the calling
workflow does not need a checkout step and every check below sees the repository.
Several of the sub-actions also check out for themselves; a repeat checkout of
the same repository and ref is idempotent.
