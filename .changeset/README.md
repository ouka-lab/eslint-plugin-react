# Changesets

Add a changeset to a PR that should appear in the release notes in `CHANGELOG.md`. CI does not require it.

```sh
pnpm changeset          # choose major / minor / patch and write the summary
pnpm changeset --empty  # for a PR that should not appear in the release notes (CI, docs, ...)
```

See [the Changesets docs](https://github.com/changesets/changesets/blob/main/docs/adding-a-changeset.md) for details.
